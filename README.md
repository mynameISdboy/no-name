# WebView Android Browser

A small Android browser with URL/search navigation, JavaScript, DOM storage, pinch-to-zoom, and a loading progress bar. Launcher icon and app name ("Browser") are shown plainly on the home screen — nothing about this app is hidden or disguised.

## Build options

### Option A — Cloud build (no computer needed)
See `CLOUD_BUILD.md` for step-by-step instructions to build via GitHub Actions and download the APK straight to your phone.

### Option B — Android Studio
Open this folder in Android Studio, let it generate the Gradle wrapper on first sync (or run `gradle wrapper` yourself if you have Gradle installed), then:
Build > Build Bundle(s) / APK(s) > Build APK(s)

The debug APK will be under:
`app/build/outputs/apk/debug/app-debug.apk`

## Install
Transfer the APK to your Android phone and open it. Android will prompt you to allow installation from whichever app you used to open the file.
