# Utility Hub

Windows utilities with one launcher and a choice of apps on each PC. This repository hosts installers, release notes and update metadata. Application source code is maintained separately.

**[Get the latest release](https://github.com/carrnate85-stack/utility-hub-updates/releases/latest)**

Current 4.2.0 installer: [Download setup](https://github.com/carrnate85-stack/utility-hub-updates/releases/download/v4.2.0/Utility-Hub-Suite-Setup-4.2.0.exe). For later versions, use the latest-release page above to find their setup file.

## Install

1. Use Windows 10 or 11, 64-bit, with the [Microsoft Edge WebView2 Evergreen Runtime](https://developer.microsoft.com/en-us/microsoft-edge/webview2/) installed. Choose the x64 runtime if you need its standalone installer.
2. Download and run the setup file. This first release is unsigned; publisher code signing is not configured.
3. Choose the utilities you want. Utility Hub is required; all eight utilities start unchecked on a new PC.
4. Open your selected apps from the Start menu.

Available utilities: **QuickExtract, Browser Guard, PDF Reader, Privacy Sweep, Quick Capture, QuickHealth, QuickText and TextReader**.

Setup remembers this PC's choices for future upgrades. Rerun it to add or remove utilities. Unchecking an installed utility removes its application files while retaining saved data. Close suite apps before updating; Setup will ask you to close running apps or release locked files. It does not force them to stop.

Documents, settings, snippets and browser profiles stay in your Windows user profile. Uninstall preserves personal data and files it does not own.

Browser Guard requires a separate manual step: open its setup app and follow the instructions to activate the included extension in Edge or Chrome. Movies and Live Sports are separate applications and are not included in this installer. Browser Guard Passwords also has a separate release.

## Updates

The installer includes `carrnate85-stack/utility-hub-updates` as its default update source. Utility Hub checks shortly after startup and about every six hours while it is running. When an update is available, it shows a notification in the Hub. **Download and installation begin only when you choose.** Updates remember the apps installed on this PC and preserve their saved data.

Open **Utility Hub → Check for updates** to check manually or change the source. For an earlier local build, enter `carrnate85-stack/utility-hub-updates` in **GitHub release source** and choose **Save source**. You can turn automatic checks off there.

## Release files

Use the setup executable for app selection. The optional portable ZIP contains the full suite. Each release includes `SHA256SUMS.txt` and `QuickSuite-Updates.json`; the Hub verifies the installer checksum before opening it.

The first release passed isolated app and installation tests. Execution on a separate physical PC or clean Windows virtual machine has not yet been verified.
