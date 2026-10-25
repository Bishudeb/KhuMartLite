# KhuMart Lite — GitHub Actions APK Demo

This repository builds the Flutter app in `app/` into debug and release APKs with GitHub Actions.

## Run a demo build
1. Upload/extract the contents of the `khumart` project ZIP into this repository so `.github/`, `app/`, `backend/`, `docs/`, and `README.md` are visible at the repository root.
2. Open **Actions → Build KhuMart APK**.
3. Select **Run workflow** and branch **main**.
4. Open the completed run, then download the **khumart-apk** artifact.

The first build may expose Flutter/Dart compatibility errors that need fixing. An APK is not available until the workflow completes successfully.

Default demo store URL: https://web.netoday.in
To change it, set repository variable `KHUMART_SITE` under Settings → Secrets and variables → Actions → Variables.

The workflow's release APK is intended for testing unless a production signing key is configured. Never commit signing keys or passwords to the repository.
