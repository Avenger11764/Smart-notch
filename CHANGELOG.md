# Release notes

## 7.2.0 — submitted to Microsoft Store

The first update since 7.1.12 (7.1.13 was not released; its changes are included here).

- **System stats in one place.** CPU, memory, network, storage, battery and uptime now share a single System stats view (the separate Network page is gone). Each tile shows the live number with a small graph or bar, and turns red when usage is very high. Choose exactly which tiles appear in Settings → Widgets → System stats; your choice also applies to the dashboard and Bar mode.
- **Better on desktop PCs.** PCs without a battery no longer show a permanent "100%, charging" ring. The closed notch's left side is now yours to choose in Settings → General → Collapsed indicator: Auto (battery on laptops, CPU on desktops), Battery, CPU usage, Memory usage or nothing.
- **Focus timer, redesigned.** A bigger timer with a progress bar, larger tasks and checkboxes, and a done count. Drag tasks by their handle to reorder them, sort them (unfinished first, A→Z, newest or oldest) or clear completed ones. The notch now stays open while you add tasks, so you can type several in a row.
- **Lyrics.** Lines glide smoothly from one to the next instead of jumping or flickering, and long lines in fullscreen no longer lose their last letters.
- **Fixed:** the green camera dot staying on after the camera was closed (some webcams stay powered even when idle), and the camera or microphone dot getting stuck after an app crashed while using it.
- **Shake to cloak (Pro)** now only reacts when you shake the pointer over the notch, pill or bar. Shaking it anywhere else on the screen no longer turns the Invisibility Cloak on.
- **Fewer "not responding" reports:** Smart Notch now closes promptly when Windows updates it, signs you out or shuts down, instead of waiting to be forced closed.
- **Settings:** new dark dropdown menus in place of Windows' grey lists, and a look at Tidy Shelf, the developer's new app for decluttering Downloads and Desktop.
- **Notchy follows your AI agents on its own (Pro).** Smart Notch now reads the session files Claude Code, Codex and Antigravity write as they work, so Notchy shows what each one is doing without installing anything in them: every step ("Reading App.jsx", "Running npm test"), every file edit with its added and removed lines (click it to see the changes), and a card with the agent's answer when it finishes. It works for sessions that were already open, and it can never block or slow down an agent.
- **Answer Claude Code from the notch.** Its questions show their choices right in the card (click one, or press 1–8); permission requests have Allow, Deny and Always (Claude Code's own "don't ask again" rule). Codex permission requests work too, after you trust Smart Notch's hooks once in Codex (`/hooks`). Cards now wait up to about two minutes for you instead of 30 seconds, and **Open terminal** brings the agent's window to the front.
- **Fixed for Notchy:** agent notifications not arriving when the Store app and another copy of Smart Notch were both installed (each rewrote the agents' settings for itself); Antigravity tools being blocked by a Smart Notch hook ("…SmartNotch.Native.exe is not recognized"), Antigravity no longer uses hooks at all; and Codex's notify setting calling Smart Notch in a loop. Notchy now shows how each agent is connected, and tells you when an agent's hooks are installed but not running.
- **Notchy** hops when a task finishes, shows a "?" when it has a question for you, and dozes after two quiet minutes.

Available through Microsoft Store once certified. Update availability can vary by device and market.

## 7.1.12 — released

- **New (Pro): Edge Light.** One tap on the dashboard (next to Customize in Quick Launch) puts a bright band around your screen to light your face on video calls, like the Mac's Edge Light. The top row with window buttons and the taskbar stay clear, the band ignores clicks, and the screen goes to full brightness while it's on (back to normal after). Adjust its width and its warmth, from cool blue through white to warm yellow, with the arrow next to the button. Settings → Widgets → Edge Light hides the button.
- **One notch only:** fixed two notches appearing at the same time, most often after waking the PC from sleep (Windows could start a second copy while the first was still waking up). A second copy now closes itself within seconds, and a copy that has frozen is replaced automatically. This also fixes "Cloak hotkey unavailable" when the second copy held Ctrl+Alt+H.
- **Invisibility Cloak:** shaking the pointer now only turns the cloak on. It clears only with a click, Esc or Ctrl+Alt+H, so moving the pointer over the notch (for example after Ctrl+Alt+Del) can no longer uncover the screen.
- **Hide until hovered:** the notch and pill now finish closing and then slide out of view, the reverse of how they appear, instead of vanishing at once.
- **Opens on more PCs:** fixed "This app can't be opened" on some Windows 10 PCs (for example Windows 10 IoT Enterprise LTSC 2021). Windows blocked the Vulkan graphics file `vulkan-1.dll` and then marked the whole app as damaged; Smart Notch draws with Direct3D and no longer includes or loads Vulkan.
- **Fewer freezes and crashes:** the crash-reporting helper process, which Windows was reporting as frozen, is gone, and the software graphics fallback (SwiftShader) that crashed on some PCs is no longer used.
- **Custom wallpaper:** choose whether it shows only when the notch is open or on the closed notch too (Settings → Appearance → Custom wallpaper). Wallpapers and background effects now also fill the two small curved corners where the notch meets the top of the screen, instead of leaving them black.
- **Polish:** the new Smart Notch icon in the taskbar, tray and Settings; no faint band left at the top of the screen when "hide until hovered" hides the notch; and changing a setting from inside the open notch no longer freezes it.
- **Full-screen detection:** the notch no longer disappears behind ChatGPT, Discord, VS Code and other maximized apps when the taskbar is set to auto-hide. It still hides for real full-screen games, videos and F11 browsers.

Available through Microsoft Store once certified. Update availability can vary by device and market.

## 7.1.11 — released

- **Shake to cloak (Pro):** shaking the pointer over the notch now toggles the Invisibility Cloak right away and every time, on every mouse and touchpad. Previously it could react late or not at all on high-precision touchpads and gaming mice, at display scaling above 100%, or when the shake swung past the edge of the notch.

## 7.1.10 — released

- **Games and full-screen apps:** Smart Notch now hides itself while a full-screen game, video or presentation covers its screen, and no longer pops open in the middle of a game. It comes back when you leave, without taking focus.
- **Always opens:** opening Smart Notch while it is already running now shows the notch and Settings instead of appearing to do nothing. If a previous copy froze, it is replaced automatically instead of blocking every launch until a restart. A start-up problem in one feature can no longer prevent the notch and tray icon from appearing.
- **Fewer freezes:** copying from busy apps (for example a large Excel selection), switching to a window that is not responding, and files on offline network shares, OneDrive online-only files or sleeping USB drives can no longer freeze Smart Notch.
- **Graphics stability:** if the graphics driver crashes repeatedly, Smart Notch starts in a safe software-rendering mode for a few days instead of closing.
- **Troubleshooting:** Settings → About → Troubleshooting now opens the real log and crash-dump folders (previously Windows reported "Location is not available").
- Fixed dragging files out of the Drop Shelf, the blank tray icon, and a downloads folder from the developer's PC being checked on every computer.

## 7.1.9 — released

- **New (Pro): Invisibility Cloak.** Off by default — turn it on in Settings → Widgets. Then press Ctrl+Alt+H (or, with Shake to cloak enabled, shake the pointer left and right inside the open notch) to frost every window behind a privacy blur. Press Ctrl+Alt+H again, click anywhere or press Esc to clear it.
- Midnight Liquid now uses the same dark molten-liquid effect as the Smart Notch website and fills the whole notch.
- Compact Pro dashboard: cards sit closer together, nothing scrolls and the notch is smaller.
- Fullscreen music: click the cover to flip it and see which app is playing; the Visualizer button cycles Waves, Bars, Ring, Mirror and Particles.
- Synced lyrics follow the song smoothly and switch lines on time, using less processor time.
- The side-notch dashboard fits completely, with a compact Quick Launch icon row.
- Open at sign-in works reliably and your choice is kept; if Windows has Smart Notch disabled in Startup apps, the app explains how to turn it back on.
- Notchy agent notifications: each agent has its own Notchy colour (Claude orange, Antigravity/Gemini blue, Codex green, Cursor indigo, Git pink), and hooks are re-connected automatically after updates.
- Bars adapt to their size: shrinking a bar hides secondary details instead of cutting features off.
- Stability: unexpected errors no longer close Smart Notch, a frozen notch recovers automatically, memory is kept in check and start-up at sign-in is lighter.
- Bar and Pill: closed notifications no longer leave an invisible area that blocks clicks under the notch, auto-hide bars no longer stay hidden, the side-bar clipboard opens beside the bar instead of over it, and damaged layout settings recover automatically.
- Fixed clipped media text in the Pro dashboard and dragging Shelf files to folders, the desktop and other apps.
- Agent completion notifications dismiss automatically; approval requests still require a response.
- Added Settings → About → Troubleshooting shortcuts to local logs and crash dumps, without automatic uploads.

Available through Microsoft Store. Update availability can vary by device and market.

## 7.1.8 — released

- Replaced background PowerShell hardware helpers with native Windows operations.
- Improved download monitoring, clipboard handling and background worker recovery.
- Improved window cleanup and positioning when display settings change.
- Added local crash and responsiveness diagnostics to help investigate failures.
- Fixed clipped text in notification cards.

Available through Microsoft Store. Update availability can vary by device and market.

## 7.1.7 — released

- Improved window-preview responsiveness and fixed a desktop-handle leak.
- Fixed enlarged side-notch panels extending beyond the screen.
- Fullscreen music centers artwork and controls when synced lyrics are unavailable.
- Added a 12-hour / 24-hour clock choice below Style in General settings.
- Improved update detection and clearer update-check messages.
- Floating pill layout with configurable distance from the screen edge.

Available through Microsoft Store. Update availability can vary by device and market.

## 7.1.6 — released

- Added Microsoft Store account ownership checks when the local Pro add-on license is missing, including for externally redeemed promo codes.
- Restore purchases now starts a fresh check after any in-progress request and retries briefly for delayed ownership updates.
- Checkout rechecks ownership after successful or already-owned results; a checkout result alone does not unlock Pro.

After updating, select **Restore purchases** using the Microsoft Store account that redeemed the Pro code.

## 7.1.5 — prepared for Store submission

- Roomier side-notch panels with larger, two-row navigation.
- Fixed clipping of music controls, including audio output and fullscreen.
- Dedicated lyrics area when the notch is on either side.
- Improved taskbar hiding for Settings and fullscreen music transitions.
- Removed the automatic copied-link popup; clipboard history remains available.
- Updated privacy disclosures for clipboard monitoring, download records and agent integrations.

The package is prepared; public Store availability is not yet confirmed. Pill mode is not part of this release.

## 7.1.0–7.1.4 — Pro rollout preparation

- One-time Microsoft Store Pro purchase and restore integration.
- Notchy, desktop screens and agent integrations.
- Free/Pro dashboard and clipboard refinements.
- Notch/bar layout fixes and audio-resource cleanup.

Subsequent builds corrected Store checkout integration and improved the Pro purchase interface and licensing notices. Free acquisition, restoration and Pro features were tested through a private Store flight. This does not confirm availability in every market or constitute a paid-charge test.

## Earlier versions

See the Microsoft Store listing for the version currently offered to your device. The public update feed advertises the latest released version.
