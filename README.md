## Quick overview
- [General information ](#general-information)
  - [Architecture](#architecture)
- [File structure](#file-structure)
- [VIPER overview](#viper-overview)
- [VIPER detailed](#viper-detailed)
- [Other modules description](#other-modules-description)

## General information
### Architecture
Core approach for skeleton architecture is [VIPER](https://github.com/strongself/The-Book-of-VIPER).
### Network communication
App use web socket for connection and custom data transfer protocol for parsing bytes from socket.  
### Security
For handshake used RSA cryptography, and AES for session token.
### UI
Layout interface programmatically [Snap Kit](https://github.com/SnapKit/SnapKit) instead using storyboard. Tables are made with [SpreadsheetView](https://github.com/kishikawakatsumi/SpreadsheetView).
