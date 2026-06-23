Cloud APK Build Ready

This project includes a GitHub Actions workflow at:
.github/workflows/build-apk.yml

It builds a debug APK in the cloud and uploads the APK as an artifact.
No local Android Studio / Android SDK installation is required.

Steps:
1. Create a GitHub repository.
2. Upload the project files so app/, build.gradle, settings.gradle, and .github/ are at repository root.
3. Open Actions > Build ANIK One Desk APK > Run workflow.
4. Download artifact: ANIK-One-Desk-debug-apk.
5. Extract and install app-debug.apk.
