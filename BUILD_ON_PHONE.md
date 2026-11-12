# DEAR AI — one-click cloud APK build

This package includes the Android source and a GitHub Actions workflow that builds a **debug APK** in GitHub's cloud runner.

## Important
- This is not a prebuilt APK. It is a build recipe.
- A free GitHub account is required to run GitHub Actions; no payment is needed for ordinary public repositories within GitHub's free usage limits.
- The output is a debug-signed APK for testing, not a Play Store release.
- It does not bypass Android Advanced Protection. If your phone blocks sideloaded APKs, do not disable security protections to force installation.
- This app is still a basic voice-command prototype, not an unrestricted AI assistant or always-listening wake-word app.

## Build using only your phone's browser
1. Download this ZIP and extract it using your phone's built-in Files app.
2. In Chrome, open https://github.com and sign in or create a free account.
3. Create a **new public repository** named `dear-ai-android`.
4. Upload the extracted project files and folders to the repository root. Make sure `.github/workflows/android-apk.yml` is included.
5. Open the repository's **Actions** tab and enable Actions if prompted.
6. Select **Build DEAR AI APK** on the left, tap **Run workflow**, then confirm.
7. Wait for the workflow to finish successfully.
8. Open that workflow run, scroll to **Artifacts**, and download `DEAR-AI-debug-APK`.
9. Extract the artifact ZIP; it contains `app-debug.apk`.

If the build fails, open the failed run and share the error log; do not try to install a failed or unrelated APK.
