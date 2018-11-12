# STARBASE ALPHA

Initial considerations for the Starbase Alpha Manual with proposed names and description for the initial release components.

## DESCRIPTION
Starbase Alpha is a collection of software written in JavaScript for Node.js and the Web. The components are small, simple to use APIs and libraries for storing, managing and transmitting data between the server and the browser client. The project serves as a platform for prototyping and building progressive web applications with secure, offline-first funtionality.

## RESOURCES

 - Starbase Alpha Manual
 - Starbase Data Storage API Specification
 - Starbase Channels API Specification

## STORAGE ENGINES / DATA STORES
Starbase Storage Engines are key-value data stores that provide the storage and basic CRUD operations according to the Data Storage API Specification. To be considered "spec-complete" the engine must provide the basic CRUD and management operations and conform to the data input/output parameters as outlined in the specification.

The Data Storage API Specification is not a database itself. It is a specification for implementing a data store. Any underlining database or storage medium that can store and retrieve data according the specification can be used to implement a storage engine.

All "spec-complete" storage engines provide an export method for exporting the data in a manner that can in turn be imported directly into another "spec-complete" storage engine with a corresponding import method.

The persistance of the data and medium by which the data is stored by the storage engine is irrelevant to the specification. To clarify, the spec does not outline how the storage engine data is stored and retrieved, or for how long it persists. The spec only outlines the required methods (functions) that the storage engine must implement, the parameters that each required method must accept, and the expected result of each required method.

### Memory Storage Engine (memstore)
The Memory Storage Engine (memstore) stores data in memory and functions as a data store on Node.js and in the browser. When used in a Node.js application, the data will persist until the application stops or is terminated. In the browser, the data persists until the window/tab is refreshed or closed.

Memory storage is suitable for temporarily storing and managing data in memory. One use case is storing data in the browser that is then displayed to the user. Changes can be made to the memory store data and then exported and saved in a more permanent storage engine or discarded. On the server, a memory store could be used as a cache for frequently accessed data.

Memory stores can write (and often access) data faster than permanent storage engines with some important limitations to consider. The amount of physical memory available to the server or browser should be considered when storing and accessing data from a memory store. Large datasets (many MBs in size) can be slow or sluggish depending on the resources available to the application. It is best to store large amounts of data in a permanent storage engine and use memory storage for caching and managing smaller sets of data.

### Web Storage Engine (webstore)
The Web Storage Engine (webstore) is built for the browser and is the original model for the other storage engines. Data is stored within an IndexedDB store that shares the name of the IndexedDB database it lives within. Data persists between browser sessions. The API for accessing the webstore is simple compared to the standard IndexedDB API. The desire for an easy way to store and access IndexedDB was the motivation behind this library.

The webstore is suitable for storing relatively large amounts of data in the browser that needs to persist between browser sessions. The webstore can be useful for storing fetch results from an external API, and then loading them again on a browser refresh, rather than making a network request back to the external API for the same data.

The webstore does not use, leverage, or even acknowledge IndexedDB indexes. It treats the database as a key-value store. Other limitations of the webstore can vary depending on the web browser. In general, there is a maximum amount of space that the web browser will allow for each IndexedDB database. In some cases, exceeding that amount may cause the browser to prompt the user to raise the limit, or may even delete old data to make room for new data. If the user clears their browser history and cache, this can also remove the data. Treat the webstore as a "mostly" persistant data store.

### Database Storage Engine (dbstore)
The Database Storage Engine uses LevelDB as the underlining storage mechanism and is suitable for permanent persistant storage on a Node.js server. This data store was built as a companion to the client-side webstore to allow for the server and client to syncronize data between each other and share the same overarching database structure.

The dbstore provides a key value store in Node.js applications can be be used for persistant storage in express APIs. Like the memstore and webstore, the dbstore shares the same CRUD and management operations, as well as database OPEN and CLOSE methods. This can be useful on the server side if an application needs access to multiple databases that may need to be opened, used, and then closed when no longer needed.

The dbstore shares the limitations of LevelDB. Data can be written very fast, and even faster in batch operations. Limited range queries can also be very fast. It is said that LevelDB is not as efficient at requesting random individual keys. While this limit exist, in my personal experience I have not found it to be an issue. In some cases, there is a possibility of data loss should uncommitted writes be lost in the event of low memory or a sudden application termination.

## DATABASE / CHANNELS

### Starbase Channels (agnostic)

### Starbase Database (proposed)

## CLIENT API LIBRARIES

### Rules Engine (agnostic)

### Web Request API (fetch api)

### Node Request API (request package)

### Channels API (fetch / request)

## REALTIME

### Starbase Socket (websockets)

## FUSION
