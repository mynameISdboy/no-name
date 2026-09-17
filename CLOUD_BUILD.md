# Browser — Cloud Build

This repository is configured to build the Android APK in GitHub Actions, so Android Studio is not required.

## Phone-only workflow

1. Create a GitHub account if you don't already have one.
2. Create a new repository and upload this entire project folder to it (including the `.github` folder).
3. Open the repository's **Actions** tab.
4. Select **Build Android APK**.
5. Click **Run workflow**.
6. When the workflow finishes, open the run and download the `Browser-debug-apk` artifact (a zip containing the `.apk`).
7. Unzip it on your phone (or unzip on a computer and transfer the `.apk` file to your phone).
8. Open the `.apk` file and follow Android's installation prompts. You may need to allow installs from whichever app you use to open it (Settings > Apps > Special access > Install unknown apps).

## Notes

- The workflow uses Gradle directly (via `gradle/actions/setup-gradle`), so you do **not** need to check in a Gradle wrapper (`gradlew`) — the project builds as-is.
- This produces a **debug** build, which is fine for installing on your own device but is not signed for distribution (e.g., the Play Store).
- The app requests only the `INTERNET` permission, needed to load web pages.
