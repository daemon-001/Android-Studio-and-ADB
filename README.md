# Android Studio Initial Setup

## Step 1: Download Android Studio
- Visit the official Android Studio website: [https://developer.android.com/studio](https://developer.android.com/studio)
- Click on **Download Android Studio**.
- Accept the terms and conditions.
- Download the appropriate version for your operating system (Windows, macOS, Linux).

## Step 2: Install Android Studio
1. Run the downloaded `.exe` file.
2. Follow the setup wizard and select necessary components.
3. Click **Next** and install Android Studio.

## Step 3: Initial Configuration
- Open Android Studio.
- Follow the setup wizard to download SDK components.
- Select the recommended settings.
- Install the latest **Android SDK**, **Emulator**, and necessary tools.

## Step 4: Verify Installation
- Open Android Studio and create a new project.
- Ensure the emulator or physical device runs successfully.
- Verify that **Flutter**, **Kotlin**, or **Jetpack Compose** (if applicable) are installed properly.

## Step 5: Set Up Environment Variables (Optional)
If needed, add Android SDK path to environment variables:
Find Your Android SDK Path

### 1. Open Android Studio.
- Go to File > Settings > Appearance & Behavior > System Settings > Android SDK.
- Copy the SDK Location (e.g., `C:\Users\YourUser\AppData\Local\Android\Sdk`).

### 2. Open Environment Variables
- Press Win + R, type sysdm.cpl, and press Enter.
- Go to the Advanced tab and click Environment Variables.

### 3. Add a New System Variable
- Click New under System Variables.
- Set the Variable Name as `ANDROID_HOME` or `ANDROID_SDK_ROOT`.
- Set the Variable Value to the SDK path you copied earlier.

Click OK to close all windows.
Restart your computer for changes to take effect.

## Step 6: Install Flutter (If Required)
- Download Flutter from [flutter.dev](https://flutter.dev/)
- Add Flutter to the system `PATH`.
- Run `flutter doctor` to verify the setup.

## Troubleshooting
- If you encounter errors, check logs in **Help > Show Log in Explorer/Finder**.
- Update SDK tools via **SDK Manager**.
- Ensure Java (JDK) is installed.

Now you are ready to develop Android apps in Android Studio!
