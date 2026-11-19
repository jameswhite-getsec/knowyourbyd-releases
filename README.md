# KnowYourBYD

A home screen and car control app for the **BYD Shark 6**, made by [Get Secured](https://getsecured.com.au).

**Latest version: 1.1.3** · [What's new](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases/tag/v1.1.3) · [All versions](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases)

## Download

| Download | Use it for |
| --- | --- |
| **[Installer for Mac](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases/download/v1.1.3/KnowYourBYD-Installer-Mac-1.1.3.zip)** | First install from a Mac (macOS 12 or later) |
| **[Installer for Windows](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases/download/v1.1.3/KnowYourBYD-Installer-1.1.3.zip)** | First install from a Windows PC |
| [KnowYourBYD-1.1.3.apk](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases/download/v1.1.3/KnowYourBYD-1.1.3.apk) | The app on its own, if you install by hand |
| [KnowYourBYD-helper-1.1.3.apk](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases/download/v1.1.3/KnowYourBYD-helper-1.1.3.apk) | The helper that reopens the app when the car wakes (the installers add it for you) |
| [SHA256SUMS.txt](https://github.com/jameswhite-getsec/knowyourbyd-releases/releases/download/v1.1.3/SHA256SUMS.txt) | Checksums for the files above |

Most people only need the installer for their computer. It downloads the app itself, and next time reuses that download if it's still the latest.

## First install

You need a Mac or Windows PC on the same Wi-Fi as the car (a phone hotspot works). An iPhone or iPad can't do the first
install. After that the app updates itself and you don't need a computer.

1. **Park the car**, switch it on, and connect it to the same Wi-Fi as your computer.
2. **Turn on ADB in the car.** You only do this once:
   1. On the car screen, go to **Car › System › Version**.
   2. Tap the words **Factory Reset** quickly, about 10 times. Tap the words, not the Reset button. Nothing is reset.
   3. In the menu that opens, press **Connect USB to enable debugging mode**. If some options are missing, rotate the
      screen to portrait, then back to landscape when you're done.
3. **Run the installer** on your computer:
   - **Mac:** unzip the download and double-click **KnowYourBYD Installer**. The first time, macOS blocks it because it
     isn't notarised by Apple: open **System Settings › Privacy & Security**, scroll down, click **Open Anyway** and
     confirm. A Terminal window shows each step and asks its questions there.
   - **Windows:** unzip the download and double-click **Install KnowYourBYD.bat**.
4. **Tap Allow on the car** when it asks *Allow USB debugging?* Tick *Always allow from this computer* first.
   The installer finds the car (or asks for its IP address: on the car, **Settings › Wi-Fi**, tap the connected
   network), installs the app and its helper, and opens it.
5. **Make it your home screen:** press **Home** on the car and choose **KnowYourBYD**, then **Always**.

The car's own BYD home screen stays installed, so you can switch back at any time.

## Updates

In the app, open **Settings › Updates** and tap **Check for updates**, then **Install update**. The app also checks by
itself every few hours. From version 1.1.1, if USB debugging is off, the app turns it on for the install and off again
about a minute after it reopens. If you are on 1.1.0 or earlier, turn on USB debugging in **Quick controls** before
installing.

## Check a download

Every APK is signed with the KnowYourBYD release key. The app refuses updates signed with anything else, and so does
the Mac installer. Certificate SHA-256:

`54:59:63:41:30:B1:F0:E3:2A:2A:83:65:89:59:58:34:B9:22:FD:C4:75:6B:43:93:54:CE:7C:5E:4B:77:A7:8B`

To check one yourself: `apksigner verify --print-certs KnowYourBYD-1.1.3.apk`

## Support and licence

Questions or faults: info@getsecured.com.au. In the app, **Diagnostics** makes a report you can send us.

KnowYourBYD is free software under the GNU GPL v3, with no warranty. The source code is available on request from
info@getsecured.com.au. It is an unofficial app, not made or endorsed by BYD.
