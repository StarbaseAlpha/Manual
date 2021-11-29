# Starbase Alpha Software Manual

Starbase Alpha is a collection of software written in JavaScript for Node.js and the Web. The core libraries provide APIs for storing, managing, and transmitting data between the server and the browser client. The project serves as a platform for building microservices and progressive web applications with secure, offline-first funtionality and the potential for secure, Peer-to-Peer communication when available.

- [Starbase Database Manual](#Database)
- [Starbase Channels Manual](#Channels)
- [Starbase Channels Client Manual](#Client)
- [Starbase Rules Engine Manual](#TheRules)
- [Starbase Socket Manual](#Socket)
- [Starbase Encryption Manual](#Encryption)
- [Starbase Progressive Web App Manual](#PWA)
- [Starbase Authentication Manual](#Auth)
- [Starbase Database Admin Manual](#Admin)
- [Starbase User Profiles Manual](#Profiles)
- [Starbase Libraries Manual](#Starbase)


## Manuals

<a name="Database"></a>
### [Starbase Database Manual](https://github.com/StarbaseAlpha/Database)

Starbase Database is a key-value data store for storing, accessing, and transferring data and building modern progressive web applications. Starbase Database is powerful, portable, lightweight and fast. With an easy to use API, the database removes the complications involved with underlining storage mechanisms. Starbase Database also serves as the model for building compatible APIs in other key-value stores.

 - IndexedDB Web Database
 - LevelDB NodeJS Database
 - Google Cloud Firestore Integration
 - In-Memory memstore
 - Import/Export Functionality
<br>


<a name="Channels"></a>
### [Starbase Channels Manual](https://github.com/StarbaseAlpha/Channels)

Starbase Channels Database adds a unix-like directory structure to the Starbase Database (or an API-compatible key-value store) and handles the creation and removal of parent and child documents based on channel paths. This allows for documents (channels) with sub-documents, which in turn can have child documents of their own. Channels is great for building APIs based on a path structure.

- Database Channels
- Unix-like database path structure
- Documents with sub-documents
- Channels Client API Library
<br>

<a name="Client"></a>
### [Starbase Channels Client Manual](https://github.com/StarbaseAlpha/Client)

Starbase Client is a web client for interfacing with services build with Starbase Channels on the backend. The client integrates with services such as Starbase Authentication, Starbase Database Admin, and Starbase Profiles. It can also work with custom services built using the Starbase Rules engine, or some custom implementation.

- Client for accessing remote Database Channels
- Client API Library for Node.js and the Web
- Integrates with Starbase Auth for token support
- Interfaces with Starbase Rules Engine
<br>


<a name="TheRules"></a>
### [Starbase Rules Engine Manual](https://github.com/StarbaseAlpha/TheRules)

- The Rules Engine
- Build APIs based on request paths
- Uses rules to control access to resources
<br>


<a name="Socket"></a>
### [Starbase Socket Manual](https://github.com/StarbaseAlpha/Socket)

- WebSocket Server
- WebSocket Web Client
- Handles ping/pong
- Simple API for exchanging JSON data
- Realtime communication between the browser and server
<br>


<a name="Encryption"></a>
### [Starbase Encryption Manual](https://github.com/StarbaseAlpha/Encryption)

Starbase Encryption provides secure end-to-end encrypted messaging services. The encryption scheme is based on Signal's Triple Diffie-Hellman key exchange and Double Ratchet Algorithm for handling message keys.

- More information coming soon!
<br>


<a name="PWA"></a>
### [Starbase Progressive Web App Manual](https://github.com/StarbaseAlpha/PWA)

- Simple Progresive Web App integration
- Install and Update functionality
- Service Worker Resource Caching
- Offline support
<br>


<a name="Auth"></a>
### [Starbase Authentication Manual](https://github.com/StarbaseAlpha/Auth)

- Starbase Authentication
- Built for node.js and the web
- Server and client API
<br>


<a name="Admin"></a>
### [Starbase Database Admin Manual](https://github.com/StarbaseAlpha/Admin)

- Starbase Database Administration
- Custom rules and options
- Server and client API
<br>


<a name="Profiles"></a>
### [Starbase User Profiles Manual](https://github.com/StarbaseAlpha/Profiles)

- Starbase User Profiles
- Built with Starbase Channels and Authentication
- Server and client API
<br>


<a name="Starbase"></a>
### [Starbase Libraries Manual](https://github.com/StarbaseAlpha/Starbase)

- All the Starbase Libraries in a single package
<br>


## Author
Hello, my name is Mike. I'm happy that you are taking an interest in my work. There is more to come and some major updates to the projects in the works. As always, I welcome anyone to try the code for themselves and provide feedback on their experience.

Last updated: 28th of November, 2021


