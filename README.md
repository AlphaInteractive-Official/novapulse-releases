# NovaPulse Production Application Releases & OTA Bundles

This repository hosts official production release packages, version metadata, and over-the-air (OTA) updates for the NovaPulse Android application.

## Distribution Architecture
- **Raw Core Codebase**: Securely maintained in private internal repository (`NovaPulse-Engine`).
- **Public Assets**: Only cryptographically hashed, minified, production-compiled binaries and application bundles are distributed through this repository.
- **Client Synchronization**: Whenever an Android device running NovaPulse is online, it queries `version.json` and automatically hot-reloads updated client assets without requiring an APK reinstallation.
