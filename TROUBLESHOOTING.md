# Reporting crashes or freezes

Include your Smart Notch version, Windows build, the action you were performing and whether the app closed or stopped responding.

Starting with version 7.1.9 (available in Microsoft Store), open **Settings → About → Troubleshooting** to find local logs and crash dumps.

Logs can help identify renderer, GPU and background-process failures. Crash dumps may contain personal information from memory. Nothing is uploaded automatically. Do not post dumps, unreviewed logs, credentials or your entire app data folder in public GitHub issues. Ask the developer for a private sharing channel first.

For a permanent freeze, logs may not capture the blocked operation. A process dump captured before closing the app can help investigate it, but also needs private handling. Reports and diagnostics do not guarantee an exact cause for every failure.

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
