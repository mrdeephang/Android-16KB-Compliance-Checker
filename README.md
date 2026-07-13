# Android 16KB Page Size Compliance Checker

Google requires all apps targeting Android 15+ (API level 35 or higher) that use native C/C++ code to support 16 KB memory page sizes. Check if your Android app is compatible.

## What's This About?

Google requires all Android apps on Google Play to **support 16KB page sizes**. This script checks if your app is ready.

---

## Quick Start

### 1. Create checkScript.sh in your root directory

### 2. Make the script executable

**Linux/macOS:**

```bash
chmod +x checkScript.sh
```

**Windows (Git Bash/WSL):**

```bash
chmod +x checkScript.sh
```

**Windows (PowerShell):**

```powershell
# No chmod needed, run directly with bash
```

### 3. Run it on your APK

**Linux/macOS:**

```bash
./checkScript.sh build/app/outputs/flutter-apk/app-release.apk
```

**Windows (Git Bash/WSL):**

```bash
./checkScript.sh build/app/outputs/flutter-apk/app-release.apk
```

**Windows (PowerShell):**

```powershell
bash checkScript.sh build/app/outputs/flutter-apk/app-release.apk
```

**For AAB (App Bundle):**

```bash
# Build APK first
flutter build appbundle

# Then check
./checkScript.sh build/app/outputs/bundle/release/app-release.aab
```

**That's it.** The script will tell you if you're good to go or what needs fixing.

**Test Now. Don't wait.**
