# Gallery

Android photo and video gallery app built with Kotlin, Jetpack Compose, and Material 3.

[![Build APK Release](https://github.com/SHNWAZX/Gallery/actions/workflows/build-apk-release.yml/badge.svg)](https://github.com/SHNWAZX/Gallery/actions/workflows/build-apk-release.yml)
![Latest Release](https://img.shields.io/github/v/release/SHNWAZX/Gallery?include_prereleases&label=release)
![Downloads](https://img.shields.io/github/downloads/SHNWAZX/Gallery/total?color=%23247EE0&label=downloads)
![License](https://img.shields.io/github/license/SHNWAZX/Gallery?color=%23247EE0)

![Gallery preview](./screenshots/preview.png)

## Download

Get the latest APK files from the GitHub Release:

[Download Gallery APK](https://github.com/SHNWAZX/Gallery/releases/tag/v4.2.1-42101-apk)

Recommended for most phones:

- [arm64-v8a phone ZIP](https://github.com/SHNWAZX/Gallery/releases/download/v4.2.1-42101-apk/Gallery-4.2.1-42101-arm64-v8a-phone-debug.zip)

Other builds:

| File | Use this for |
| --- | --- |
| `arm64-v8a-phone-debug.zip` | Most modern Android phones |
| `armeabi-v7a-phone-debug.zip` | Older 32-bit Android phones |
| `x86_64-emulator-debug.zip` | Android emulator on PC |
| `universal-debug.zip` | Any supported CPU, larger download |

After downloading a ZIP, extract it and install the `.apk` inside it.

## Features

- Timeline and album browsing for photos and videos
- Grid and mosaic layouts
- Material 3 interface with theme customization
- Favorites, trash, metadata, search, and media viewer tools
- Optional maps/location media views
- Optional AI model support for smart media features
- Vault features for private media workflows

## Build

This project uses Gradle and the Android SDK.

```powershell
.\gradlew.bat :app:assembleArm64-v8aNoMLDebug
```

To build without map features:

```powershell
Set-Content app.properties "INCLUDE_MAPS=false`nALL_FILES_ACCESS=true"
.\gradlew.bat :app:assembleArm64-v8aNoMLDebug
```

GitHub Actions can build release assets automatically:

- [Build APK Release](https://github.com/SHNWAZX/Gallery/actions/workflows/build-apk-release.yml)
- [Emulator Smoke Test](https://github.com/SHNWAZX/Gallery/actions/workflows/emulator-smoke-test.yml)

## Repository

The app package used by debug builds is `com.dot.gallery.debug`.

The public APKs in this repository are debug-signed test builds. For production publishing, create a private Android signing key and configure release signing secrets in GitHub Actions.

## Credits

This project is based on ReFra by IacobIonut01 and keeps the original Apache-2.0 licensed codebase structure while rebranding this fork as Gallery.

## License

Licensed under the Apache License 2.0. See [LICENSE](./LICENSE).
