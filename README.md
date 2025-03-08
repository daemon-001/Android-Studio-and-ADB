# Android Studio Setup Guide

## Step 1: Download Android Studio
- Visit the official Android Studio website: [https://developer.android.com/studio](https://developer.android.com/studio)
- Click on **Download Android Studio**.
- Accept the terms and conditions.
- Download the appropriate version for your operating system (Windows, macOS, Linux).

## Step 2: Install Android Studio
### Windows:
1. Run the downloaded `.exe` file.
2. Follow the setup wizard and select necessary components.
3. Click **Next** and install Android Studio.

### macOS:
1. Open the downloaded `.dmg` file.
2. Drag and drop Android Studio into the Applications folder.

### Linux:
1. Extract the `.tar.gz` file.
2. Open a terminal and navigate to the extracted folder.
3. Run the command:
   ```sh
   ./studio.sh
   ```

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

### Windows:
1. Go to **System Properties > Environment Variables**.
2. Add `ANDROID_HOME` or `ANDROID_SDK_ROOT` with the SDK path.

### macOS/Linux:
Add the following to `.bashrc` or `.zshrc`:
```sh
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools:$PATH
```

## Step 6: Install Flutter (If Required)
- Download Flutter from [flutter.dev](https://flutter.dev/)
- Add Flutter to the system `PATH`.
- Run `flutter doctor` to verify the setup.

## Troubleshooting
- If you encounter errors, check logs in **Help > Show Log in Explorer/Finder**.
- Update SDK tools via **SDK Manager**.
- Ensure Java (JDK) is installed.

Now you are ready to develop Android apps in Android Studio!
