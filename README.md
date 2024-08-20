# Android Customization Toolkit

Welcome to the Android Customization Toolkit!
This repository contains a collection of tools and scripts designed to help you customize your Android device with ease.
Whether you're a developer looking to modify system files or an enthusiast wanting to personalize your device, this toolkit has got you covered.

# Features
-Boot Animation Replacement: Easily replace the default boot animation on your Android device with a custom one.
-Application Management: Uninstall and reinstall system apps using ADB commands.
-Root Access Scripts: Simplify operations requiring root access with pre-configured scripts.

# Getting Started
To get started, you'll need to have ADB (Android Debug Bridge) installed on your computer and root access on your Android device.

# Prerequisites
-ADB Installation: Follow the official ADB documentation to install ADB on your system.
-Root Access: Ensure your Android device is rooted to perform system modifications.

# Usage
Replace Boot Animation:

-Pull the current boot animation: adb pull /system/media/bootanimation.zip <local_path>
-Modify the boot animation as needed.
-Push the modified animation: adb push <local_path>/bootanimation.zip /system/media/bootanimation.zip
-Set appropriate permissions: adb shell su -c 'chmod 644 /system/media/bootanimation.zip'
-Reboot your device to see the changes.

Manage Applications:

-List installed packages: adb shell pm list packages
-Uninstall a package: adb shell pm uninstall --user 0 <package_name>
-Reinstall a package: adb install <path_to_apk>

# Contact
For any questions or issues, feel free to open an issue in the repository or contact me directly.
