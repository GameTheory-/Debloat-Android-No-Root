## Backup and Debloat Android No Root v1.1
![image](configs/bnd.png)

A tool for creating backups and debloating non rooted android devices. This tool uses the adb method of backing up and uninstalling apps.

**For Android 4.0 and up**

**Tested on ubuntu & xubuntu**

**This project uses:**
- [dos2unix](https://waterlan.home.xs4all.nl/dos2unix.html)

## Limitations
Adb has its' known limitations...

1. It can only backup apps where the developer of the app allows the app to be backed up in the `AndroidManifest.xml`. In full backups those apps will be ignored. In individual app backups you will get an empty backup for those apps.
2. Apps are only uninstalled for the user and not root. This means the apps are uninstalled but remain on the device like if they are frozen (not a problem at all).

If you remove system apps that you later decide you want back, you can do a factory reset and the apps will reinstall automatically.

## Usage
Make sure the `backupdebloat` file has execute permissions.

1. Enable usb debugging on your device in developer options and then plug it to your computer.
2. Execute the file as follows in a terminal: `./backupdebloat`
3. optional - Use the "Add Desktop Shortcut" option for quick access

## Project Page
https://intechgeek.com/backup-and-debloat-android-no-root/
