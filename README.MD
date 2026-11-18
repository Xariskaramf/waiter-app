# Waiter App

An Android ordering assistant for a whiskey bar, intended to replace handwritten
order notes. The app is designed to work offline, without printers, cash registers,
or cloud integrations.

## Stack

- Kotlin and Jetpack Compose
- ViewModel and Room (SQLite), with KSP
- Minimum Android 6.0 (API 23); target SDK 36

## Status

Initial skeleton with a welcome screen and light/dark theme.
Order management, database tables, backups, and device synchronization are not
implemented yet.

## Run

1. Open the repository in Android Studio.
2. Use JDK 17 or 21 and install Android SDK Platform 36 / Build-Tools 35.0.0.
3. Sync Gradle and run `app` on an emulator or Android device.

The first build requires internet access to download dependencies.

## Build and lint

macOS/Linux:

```sh
./gradlew :app:assembleDebug :app:lintDebug
```

Windows PowerShell:

```powershell
.\gradlew.bat :app:assembleDebug :app:lintDebug
```

Debug APK: `app/build/outputs/apk/debug/app-debug.apk`.