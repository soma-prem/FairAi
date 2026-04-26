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

