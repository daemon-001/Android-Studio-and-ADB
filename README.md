# Android Studio Quick Setup

## 1. Download & Install
- Get Android Studio from [developer.android.com/studio](https://developer.android.com/studio).
- Run the installer and follow the setup wizard.

## 2. Initial Setup
- Open Android Studio → follow the wizard.
- Install SDK, Emulator, and necessary tools.

## 3. Verify Installation
- Create a new project.
- Run it on an emulator or physical device.

## 4. Set SDK Path
- Search “Environment Variables” → Edit the system environment variables
- Click Environment Variables → New (under **User** variables) then add this:
```yaml
Variable name: ANDROID_HOME
Variable value: C:\Users\<YourUser>\AppData\Local\Android\Sdk

# Add this to Path of User variables:
%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\tools
```

## 5. Verify Installation
- Run these commands in **Command Prompt** or **Terminal**:
```bash
# Check Java installation
java -version

# Check Android SDK path
echo %ANDROID_HOME%       # Windows
echo $ANDROID_HOME        # macOS/Linux

# Verify adb (Android Debug Bridge)
adb version
```

✅ **You’re ready to build Android apps!**
