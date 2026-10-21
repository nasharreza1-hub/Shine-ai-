# Shine AI — Android APK build project

This is a lightweight Android WebView wrapper around the Shine AI prototype. It can build a debug APK using GitHub Actions, without Android Studio on your phone.

## Important
- This build contains a **prototype**, not a connected online AI service or bundled offline language model.
- Chat responses are demo/scripted responses from the prototype. Voice/browser features can vary by Android WebView.
- The generated APK is a debug APK for testing, not a Play Store release.

## Build using only an Android phone
1. Download and extract this ZIP.
2. In your mobile browser, open https://github.com/new and create a repository named `shine-ai` (Public makes the setup easier; do not upload secrets).
3. Upload the extracted project files and folders to the repository root. Make sure `.github/workflows/build-apk.yml` is included.
4. Open the repository's **Actions** tab and choose **Build Shine AI APK**. Tap **Run workflow** if it hasn't started automatically.
5. When the run succeeds, open that run and download the **Shine-AI-APK** artifact. Extract it; the file is `app-debug.apk`.
6. Tap the APK to install. Android may ask you to allow installation from your browser/files app.

If the build fails, open the workflow run and share the error log so it can be fixed.
