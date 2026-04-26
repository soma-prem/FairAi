# FairAI (Android APK)

This repository currently contains a prebuilt Android release APK for FairAI.

## Contents

- `app-release.apk` - release build of the Android app

## Install

### Option A: Install on-device (sideload)
1. Copy `app-release.apk` to your Android device.
2. Open it using a file manager.
3. If prompted, allow installs from "unknown sources" for that app.

### Option B: Install with ADB (recommended for developers)
1. Enable **Developer options** -> **USB debugging** on your device.
2. Connect the device via USB.
3. Install/upgrade:

```bash
adb install -r app-release.apk
```

## Verify integrity (SHA-256)

Expected SHA-256 for `app-release.apk`:

```
B246DE3EE07044B90B2D940F34FFE002377CDD38CA8BA30A4E7129E419CEC735
```

PowerShell:

```powershell
Get-FileHash .\app-release.apk -Algorithm SHA256
```

## Troubleshooting

- **"App not installed"**: uninstall any older build first (signature mismatch can block updates).
- **"There was a problem parsing the package"**: the APK may be corrupted; re-copy or re-download.
- **Play Protect warning**: common for sideloaded APKs; proceed only if you trust the source.

## Notes

- Source code is not included in this folder at the moment; this repo is tracking the release artifact.
