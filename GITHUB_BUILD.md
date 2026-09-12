# PvZ Hardcore Android build

This source tree contains the hardcore gameplay changes plus a GitHub Actions workflow that builds an Android `arm64-v8a` APK.

## Build

1. Create a GitHub repository.
2. Upload the contents of this folder to the repository (the `.github/workflows/android-hardcore.yml` file must be included).
3. Open **Actions** → **Build PvZ Hardcore Android** → **Run workflow**.
4. When it finishes, open the workflow run and download the artifact named `pvz-hardcore-android-arm64-v8a`.

The build does not include PopCap/EA game assets. The resulting app still expects the user's own compatible PvZ GOTY resources through the normal PvZ-Portable resource importer.
