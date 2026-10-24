# Reporting crashes or freezes

Include your Smart Notch version, Windows build, the action you were performing and whether the app closed or stopped responding.

Open **Settings → About → Troubleshooting** to find local logs and crash dumps (fixed in 7.1.10; in 7.1.9 these buttons showed "Location is not available").

Because Smart Notch is a Microsoft Store app, Windows keeps its files inside the app's package folder, not in `%APPDATA%\smart-notch`. To open it manually, press **Win + R**, paste this and press Enter:

```
%LOCALAPPDATA%\Packages\Devavinash.DynamicIslandWindows_mv0cm4vwdc0m6\LocalCache\Roaming\smart-notch
```

`app-debug.log` is the log; crash dumps are in `Crashpad\reports`.

Logs can help identify renderer, GPU and background-process failures. Crash dumps may contain personal information from memory. Nothing is uploaded automatically. Do not post dumps, unreviewed logs, credentials or your entire app data folder in public GitHub issues. Ask the developer for a private sharing channel first.

For a permanent freeze, logs may not capture the blocked operation. A process dump captured before closing the app can help investigate it, but also needs private handling. Reports and diagnostics do not guarantee an exact cause for every failure.

# Smart Notch seems to do nothing when opened

Smart Notch starts with Windows and lives at the top of the screen, so it is usually already running. From 7.1.10, opening it again shows the notch and opens Settings. On older versions:

1. Look for the Smart Notch icon in the taskbar's hidden-icons area (^) and choose **Show Smart Notch** or **Settings**.
2. Hover the very top of your screen (or the edge where you placed it).
3. If nothing appears, open Task Manager, end every **Smart Notch** process, and open it again. 7.1.10 does this automatically when a previous copy has frozen.
4. Smart Notch hides itself while a full-screen game or video covers the screen (7.1.10 and later); leave full screen and it returns.

# "This app can't open" when starting Smart Notch

Windows shows this message before Smart Notch itself starts, so the app cannot log anything. It usually means Windows could not verify the Store licence or the installed package. Try these in order:

1. Open **Microsoft Store**, make sure you are signed in, go to **Library** and select **Get updates**. Install the latest version (7.1.9 or later).
2. Open **Settings → Apps → Installed apps → Smart Notch → ⋯ → Advanced options** and select **Repair**. If it still fails, select **Reset** (this clears Smart Notch settings).
3. Check your antivirus quarantine or **Windows Security → Protection history**. If a Smart Notch file was blocked or removed, restore it or allow it, then use **Repair** again.
4. Run `wsreset.exe` from the Start menu, wait for the Store to open, then try Smart Notch again.
5. Uninstall Smart Notch, restart Windows, and install it again from Microsoft Store.

If it still fails, open an issue with:

- your Windows version and build (**Settings → System → About**),
- whether you installed from the Store app, the Store website or `winget`,
- your antivirus product,
- the most recent error in **Event Viewer → Applications and Services Logs → Microsoft → Windows → AppModel-Runtime → Admin** (event ID and message only).
