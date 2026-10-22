# Release notes

## 7.1.9 — prepared for Store submission

- **New (Pro): Invisibility Cloak.** Off by default — turn it on in Settings → Widgets. Then press Ctrl+Alt+H (or, with Shake to cloak enabled, shake the pointer left and right inside the open notch) to frost every window behind a privacy blur. Press Ctrl+Alt+H again, click anywhere or press Esc to clear it.
- Midnight Liquid now uses the same dark molten-liquid effect as the Smart Notch website and fills the whole notch.
- Compact Pro dashboard: cards sit closer together, nothing scrolls and the notch is smaller.
- Open at sign-in works reliably and your choice is kept; if Windows has Smart Notch disabled in Startup apps, the app explains how to turn it back on.
- Notchy agent notifications: each agent has its own Notchy colour (Claude orange, Antigravity/Gemini blue, Codex green, Cursor indigo, Git pink), and hooks are re-connected automatically after updates.
- Bars adapt to their size: shrinking a bar hides secondary details instead of cutting features off.
- Stability: unexpected errors no longer close Smart Notch, a frozen notch recovers automatically, memory is kept in check and start-up at sign-in is lighter.
- Fixed clipped media text in the Pro dashboard and dragging Shelf files to folders, the desktop and other apps.
- Agent completion notifications dismiss automatically; approval requests still require a response.
- Added Settings → About → Troubleshooting shortcuts to local logs and crash dumps, without automatic uploads.

This package is not yet confirmed available in Microsoft Store. The update feed remains on released version 7.1.8.

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

See the Microsoft Store listing for the version currently offered to your device. The public update feed now advertises the released 7.1.8 version.
