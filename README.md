# GOLDENMC NEXUS — Official Updates

Official public distribution repository for the **GOLDENMC NEXUS** Android app.

## Download

The latest published Android release will be available here:

https://github.com/irfangameplay76-eng/GOLDENMC-NEXUS-UPDATES/releases/latest

## Release asset

Every release must include the signed APK with this exact filename:

`GOLDENMC-NEXUS.apk`

## In-app updater

The app's update manifest is hosted separately at:

https://goldenmc.ir/update.json

For each new release:

1. Build a **signed** APK using the same application ID and signing key as the installed app.
2. Increase `versionCode` above the version already published.
3. Create a GitHub Release with a version tag (for example, `v1.0.1`).
4. Attach the APK as `GOLDENMC-NEXUS.apk`.
5. Copy the exact asset download URL into the `apkUrl` field in `update.json`.
6. Update the manifest's `versionName`, `versionCode`, and Persian `releaseNotes`, then publish the manifest.

**Important:** Never publish a debug APK as an update for users, and never change the app's signing key or application ID between updates.
