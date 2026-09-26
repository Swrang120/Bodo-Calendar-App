# Bodo Calendar App

Dedicated update repository for Bodo Calendar.

## Update system

The Android app checks this repository's `version.json` for a newer `versionCode`.

Manifest:
`https://raw.githubusercontent.com/Swrang120/Bodo-Calendar-App/main/version.json`

When a newer APK is released:
1. Upload the new APK to this repository.
2. Update `version.json` with the new `versionCode`, `versionName`, release notes, and APK URL.
3. Existing app installations detect the newer version automatically.
4. The app shows its Quick Update dialog.

## Important

The APK must use the same Android application ID and signing certificate as the installed version, and its version code must be higher for a normal update.

GitHub Actions can automate Android build/test workflows when the source and signing credentials are configured.
