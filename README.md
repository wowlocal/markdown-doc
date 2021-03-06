# Documentation
---
## Quick overview
- [General information](#general-information)
  - [Architecture](#architecture)
  - [Network communication](#network-communication)
  - [Security](#security)
  - [UI](#ui)
- [File structure](#file-structure)
- [VIPER overview](#viper-overview)
- [VIPER detailed](#viper-detailed)
- [Other modules description](#other-modules-description)

## General information
### Architecture
Core approach for skeleton architecture is [VIPER](https://github.com/strongself/The-Book-of-VIPER).
### Network communication
App use web socket for connection and custom data transfer protocol for parsing bytes from socket. Socket communicates with services via RxSwift.
### Security
For handshake used RSA cryptography, and AES for session token.
### UI
Layout interface programmatically [Snap Kit](https://github.com/SnapKit/SnapKit) instead using storyboard. Tables are made with [SpreadsheetView](https://github.com/kishikawakatsumi/SpreadsheetView).

## File structure
```
├── BusinessLogicLayer
│   ├── CoreComponents
│   │   ├── Cryprography
│   │   └── Socket
│   │       └── TransferProtocol
│   │           └── Protofiles
│   └── Services
├── Helpers
│   └── TransitionHandler
├── ModelLayer
│   └── Enitites
├── Modules
│   └── TaskProcessTracking
│       ├── Assembly
│       ├── Interactor
│       ├── Presenter
│       │   └── PresenterState
│       ├── Router
│       └── View
│           └── Cells
├── Protocols
├── Resources
├── ServicesAssemblyLayer
└── Singletones
```

## VIPER overview
