# Android Tap Circle Game

This is a minimal Android Studio project that loads a small HTML5 canvas game inside a WebView.

What you get
- A simple Android app (`app` module) written in Kotlin
- `MainActivity` that loads `app/src/main/assets/index.html`
- A tiny HTML5 game: tap the moving circle to gain points before time runs out

Quick start
1. Open this project folder in Android Studio.
2. If prompted, configure the Android SDK in Android Studio.
3. Build and Run the `app` module on an emulator or physical device (API 21+).

Configuring the Android SDK (important)
- The build requires the Android SDK. Create or edit `local.properties` in the project root and set your SDK path, for example:

```text
sdk.dir=/home/username/Android/Sdk
```

- Alternatively open the project in Android Studio; it will help you configure the SDK automatically.

What I created for you
- `app/` - Android application module (Kotlin)
- `app/src/main/assets/index.html` - Playable HTML5 game (tap the moving circle)
- `app/src/main/java/com/example/androidgame/MainActivity.kt` - Kotlin activity that hosts a WebView
- Gradle files: `settings.gradle`, `build.gradle`, `app/build.gradle`, and generated Gradle wrapper files
- `local.properties` (placeholder with instructions) — please set `sdk.dir` to your SDK path

Build verification
- I generated a Gradle wrapper and attempted `./gradlew assembleDebug` in the container. The build failed because the Android SDK is not available in this environment. The project and wrapper are present and ready to build locally or in Android Studio.

Optional next steps I can implement
- Add an Android-native (Kotlin) version of the game using Canvas for better performance
- Add sounds, persistent high-score storage (SharedPreferences), and a main menu
- Add CI (GitHub Actions) to build the APK using a configured Android SDK image

If you want any of those, tell me which and I'll implement it.

License
This project skeleton is provided without a license. Let me know if you want a specific license added.