# HC Releases

Desktop companion for the **HC Utils release board**: a menu-bar app that notifies you when a
release moves between columns, lists releases by column, and opens the board in its own window.
You need a HeavyConnect Google account with access to HC Utils.

This repository only hosts the downloads and the auto-update feed.

## Install

Download the file for your system from the [latest release](../../releases/latest).

### macOS (Apple Silicon and Intel)

1. Download `HC.Releases_<version>_universal.dmg`, open it and drag **HC Releases** to Applications.
2. The app isn't notarized, so the first launch is blocked. Open it once, then go to
   **System Settings → Privacy & Security** and click **Open Anyway**.
   (Or, in Terminal: `xattr -dr com.apple.quarantine "/Applications/HC Releases.app"`.)
3. Sign in with your HeavyConnect Google account when the board window opens.

After each update macOS asks once whether HC Releases may use its saved session in the Keychain:
enter your password and choose **Always Allow**.

### Windows

Run `HC.Releases_<version>_x64-setup.exe`. SmartScreen may warn about an unknown publisher:
click **More info → Run anyway**.

### Linux

Use the `.AppImage` (make it executable) or the `.deb`. On GNOME, tray icons need the
AppIndicator extension.

## Updates

The app checks for updates at launch and daily, downloads them in the background, and shows
**Restart to update** in its menu when one is ready. Updates are signed; the app refuses
anything that isn't.
