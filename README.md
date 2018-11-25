# STARBASE ALPHA SOFTWARE MANUAL

Starbase Alpha is a collection of software written in JavaScript for Node.js and the Web. The components are small, simple to use APIs and libraries for storing, managing and transmitting data between the server and the browser client. The project serves as a platform for prototyping and building progressive web applications with secure, offline-first funtionality.

## Manuals

### [Starbase Database Manual](https://github.com/StarbaseAlpha/Database)

Starbase Database is a key-value data store for storing, accessing, and transferring data in modern, progressive web applications. Starbase Database is powerful, portable, lightweight and fast. With an easy to use API, the database removes the complications involved with underlining storage mechanisms.

 - IndexedDB Web Database
 - LevelDB NodeJS Database
 - In-Memory memstore
 - Import/Export Functionality


### [Starbase Channels Manual](https://github.com/StarbaseAlpha/Channels)

Starbase Channels adds a unix-like directory structure to the Starbase Database and handles the creation and removal of parent and child documents based on channel paths. This allows for documents (channels) with sub-documents, which in turn can have child documents of their own. Channels is great for building APIs based on a path structure.

- Database Channels
- Unix-like database path structure
- Documents with sub-documents
- Channels Client API Library


### Starbase Rules Engine Manual - Coming soon

- The Rules Engine
- Build APIs based on request paths
- Uses rules to control access to resources


### Starbase Socket Manual - Coming soon

- WebSocket Node.js Server
- WebSocket Web Client
- Simple API for exchanging JSON data
- Handles ping/pong and reconnect on disconnect
- Realtime communication between the browser and server


### Starbase Defacto Server Manual - Coming soon

- Defacto Node.js Express Web Server
- Includes helmet and compression middleware
- Optional JSON body parser and limiter
- Optional static path for public files
- Optional CORS support


### [Starbase Encryption Manual](https://github.com/StarbaseAlpha/Encryption)

Starbase Encryption provides 256-bit AES-GCM encryption with HMAC signatures and PBKDF2 password stretching in the browser and in nodeJS. The web version uses the browser's built-in Web Crypto library. The node-webcrypto-ossl package is used server-side in NodeJS.

- 256-bit AES-GCM Encryption
- HMAC signatures
- PBKDF2 password stretching
- Browser and Node.js solutions


### Starbase Reference App Manual - Coming soon

- Starbase Developer Full-Stack Reference Application
- Server-side Channels API with Rules Engine integration
- Client-side Offline-first Channels database
- Server/Client Sync


## ADDITIONAL INFORMATION

### Author
Hello, my name is Mike. I'm happy that you are taking an interest in my work.
