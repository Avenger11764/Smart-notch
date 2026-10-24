# Release notes

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
