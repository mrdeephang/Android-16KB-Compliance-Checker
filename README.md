# Android 16KB Page Size Compliance Checker

Check if your Android app is ready for Google Play's **November 1, 2025** deadline.

## Overview

<img src="https://github.com/user-attachments/assets/10f6cc2a-8263-4237-801c-234eda09cf83" alt="Android 16KB Compliance" width="600">

---

## What's This About?

Starting November 1, 2025, all Android apps on Google Play **must support 16KB page sizes**. This script checks if your app is ready.

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

**Deadline: November 1, 2025. Don't wait.**
