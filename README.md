# Starbase Alpha Software Manual

Starbase Alpha is a collection of software written in JavaScript for Node.js and the Web. The components are small, simple to use APIs and libraries for storing, managing and transmitting data between the server and the browser client. The project serves as a platform for building microservices and progressive web applications with secure, offline-first funtionality.

- [Starbase Database Manual](#Database)
- [Starbase Channels Manual](#Channels)
- [Starbase Channels Server Manual](#Server)
- [Starbase Channels Client Manual](#Client)
- [Starbase Rules Engine Manual](#TheRules)
- [Starbase Services Manual](#Services)
- [Starbase Socket Manual](#Socket)
- [Starbase Defacto Web Server Manual](#Defacto)
- [Starbase Encryption Manual](#Encryption)
- [Starbase Progressive Web App Manual](#PWA)
- [Starbase Authentication Manual](#Auth)
- [Starbase Database Admin Manual](#Admin)
- [Starbase User Profiles Manual](#Profiles)
- [Starbase Functions Manual](#Functions)
- [Starbase Libraries Manual](#Starbase)
- [Starbase Reference App Manual](#App)


## Manuals

<a name="Database"></a>
### [Starbase Database Manual](https://github.com/StarbaseAlpha/Database)

Starbase Database is a key-value data store for storing, accessing, and transferring data in modern, progressive web applications. Starbase Database is powerful, portable, lightweight and fast. With an easy to use API, the database removes the complications involved with underlining storage mechanisms.

 - IndexedDB Web Database
 - LevelDB NodeJS Database
 - In-Memory memstore
 - Import/Export Functionality
<br>


<a name="Channels"></a>
### [Starbase Channels Manual](https://github.com/StarbaseAlpha/Channels)

Starbase Channels adds a unix-like directory structure to the Starbase Database and handles the creation and removal of parent and child documents based on channel paths. This allows for documents (channels) with sub-documents, which in turn can have child documents of their own. Channels is great for building APIs based on a path structure.

- Database Channels
- Unix-like database path structure
- Documents with sub-documents
- Channels Client API Library
<br>

<a name="Client"></a>
### [Starbase Channels Client Manual](https://github.com/StarbaseAlpha/Client)

- Client for accessing remote Database Channels
- Client API Library for Node.js and the Web
- Integrates with Starbase Auth for token support
- Interfaces with Starbase Rules Engine
<br>


<a name="Server"></a>
### [Starbase Channels Server Manual](https://github.com/StarbaseAlpha/Server)

- Express web server built for Starbase Apps
- Built with Starbase Defacto Web Server
- Supports APIs built with Starbase Rules Engine
<br>


<a name="TheRules"></a>
### [Starbase Rules Engine Manual](https://github.com/StarbaseAlpha/TheRules)

- The Rules Engine
- Build APIs based on request paths
- Uses rules to control access to resources
<br>


<a name="Services"></a>
### [Starbase Services Manual](https://github.com/StarbaseAlpha/Services)

- Starbase Services
- Platform Services for building Starbase apps
- Support for Starbase Database and Starbase Starfire
- Server and Serverless (FaaS) Configurations
<br>


<a name="Socket"></a>
### [Starbase Socket Manual](https://github.com/StarbaseAlpha/Socket)

- WebSocket Node.js Server
- WebSocket Web Client
- Simple API for exchanging JSON data
- Handles ping/pong and reconnect on disconnect
- Realtime communication between the browser and server
<br>


<a name="Defacto"></a>
### [Starbase Defacto Web Server Manual](https://github.com/StarbaseAlpha/Defacto)

- Defacto Node.js Express Web Server
- Includes helmet and compression middleware
- Optional JSON body parser and limiter
- Optional static path for public files
- Optional CORS support
<br>


<a name="Encryption"></a>
### [Starbase Encryption Manual](https://github.com/StarbaseAlpha/Encryption)

Starbase Encryption provides 256-bit AES-GCM encryption with HMAC signatures and PBKDF2 password stretching in the browser and in nodeJS. The web version uses the browser's built-in Web Crypto library. The node-webcrypto-ossl package is used server-side in NodeJS.

- 256-bit AES-GCM Encryption
- HMAC signatures
- PBKDF2 password stretching
- Browser and Node.js solutions
<br>


<a name="PWA"></a>
### [Starbase Progressive Web App Manual](https://github.com/StarbaseAlpha/PWA)

- Simple Progresive Web App integration
- Install and Update functionality
- Service Worker and offline-first support
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


<a name="Functions"></a>
### [Starbase Functions Manual](https://github.com/StarbaseAlpha/Functions)

- Starbase Functions
- Isolated JavaScript Virtual Machines
- Build APIs with untrusted code
- Experimental!
<br>


<a name="Starbase"></a>
### [Starbase Libraries Manual](https://github.com/StarbaseAlpha/Starbase)

- All the Starbase Libraries in a single package
<br>


<a name="App"></a>
### Starbase Reference App Manual - Coming soon

- Starbase Developer Full-Stack Reference Application
- Server-side Channels API with Rules Engine integration
- Client-side Offline-first Channels database
- Server/Client Sync
<br>


## Author
Hello, my name is Mike. I'm happy that you are taking an interest in my work.
