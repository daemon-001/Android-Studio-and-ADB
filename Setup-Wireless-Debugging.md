# Wireless Debugging Setup for Android Development
Use a physical android device insted of emulator for debugging.

## Prerequisites
- Android Studio installed
- A device running Android 11 or higher
- Both your PC and Android device connected to the same Wi-Fi network

## Step 1: Enable Developer Options
1. Open **Settings** on your Android device.
2. Go to **About phone**.
3. Tap **Build number** **7 times** until you see "You are now a developer!".
4. Go back to **Settings** and search and open **Developer options**.

## Step 2: Enable Wireless Debugging
1. In **Developer options**, find and enable **Wireless Debugging**.
2. Tap **Pair device with QR or pairing code** (needed for initial setup).

## Step 3: Connect Your Device to ADB Wirelessly
### Option 1: Using a Pairing Code (Recommended)
1. Open a terminal or Command Prompt on your PC.
2. Run the following command to start ADB:
   ```sh
   adb pair <device-ip>:<port>
   ```
3. Enter the **pairing code** shown on your Android device.
4. Once paired, run:
   ```sh
   adb connect <device-ip>:<port>
   ```
5. Verify the connection by running:
   ```sh
   adb devices
   ```
   You should see your device listed as **"device"**.

### Option 2: Using a USB Cable (Alternative Method)
1. Connect your device to your PC via USB.
2. Run:
   ```sh
   adb tcpip 5555
   ```
3. Disconnect the USB cable.
4. Find your device's **IP address** from **Wi-Fi settings**.
5. Run:
   ```sh
   adb connect <device-ip>:5555
   ```
6. Verify the connection with:
   ```sh
   adb devices
   ```

## Step 4: Debug Your App Wirelessly
- Open Android Studio.
- Run your app on the connected device.
- Debug as usual without needing a USB cable.

## Troubleshooting
- Ensure both devices are on the same Wi-Fi network.
- Restart `adb` using:
  ```sh
  adb kill-server
  adb start-server
  ```
- Re-enable **Wireless Debugging** if the connection drops.

Now you can debug Android apps wirelessly! 🚀

