# Smart Notch Privacy Policy

**Last updated: 16 October 2026**

**Current release reviewed: Smart Notch 7.1.5 for Windows.**

This policy describes Smart Notch for Windows, including its Free features and optional Smart Notch Pro add-on, published by Dev_avinash (GitHub: Avenger11764). Features available to you depend on your installed version and settings.

## Information used by the app

Smart Notch processes information to provide desktop controls, notifications and the features you enable:

- **Clipboard:** copied text and, where supported and enabled, images, pinned items and timestamps. Clipboard contents can contain personal or sensitive information.
- **Files and downloads:** names, paths, sizes and activity information for download indicators and files you place on the Drop Shelf. The download monitor watches the local Downloads folder and can read recent download records from Chrome, Edge and Brave profile History databases to estimate progress, including target/current paths, byte counts and download state. This lookup uses the downloads table, not a list of visited web pages. Opening, copying or saving a file performs the action you request.
- **Media and system information:** track titles, artists, album artwork, playback state, audio levels for visual effects, audio/Bluetooth device names, battery status, CPU/RAM and network statistics, and microphone/camera activity indicators. Activity indicators report device usage; they are not camera video or microphone recording features.
- **Preferences and productivity data:** appearance settings, shortcuts, window positions, timers, tasks and related local state.
- **Agent and local Git integrations:** provider and account identifiers (such as email and plan), usage counters and quota resets, session/project identifiers, paths, event descriptions, and commands or permission requests supplied by an agent integration. Local Git monitoring reads information from watched repositories, including repository paths and commit or working-tree activity. Installing notification hooks changes the selected agent or repository hook configuration so it can send events to Smart Notch over a local connection. These events may include sensitive project information. Supported integrations may read local agent configuration or credentials, query a local agent service, or use the agent's signed-in account to request its usage/profile information.
- **Diagnostics:** local diagnostic logs may contain errors, paths, device details and operational events.

## Local storage and retention

Preferences and histories are stored on your device in the app's Windows user-data storage. Clipboard history is stored as a local JSON file, not as an encrypted vault. Protect access to your Windows account and avoid retaining passwords or sensitive documents in clipboard history.

The current clipboard implementation limits stored history to 50 items. Unpinned items are eligible for removal after 24 hours when the app runs its cleanup; pinned items remain until removed. Clear history preserves pinned items, so unpin or individually delete them to remove them too. Download history retains up to 30 recent records. Settings and integration configuration remain until changed or removed. Local debug logs are size-limited and rotated.

Removing a Shelf reference does not necessarily delete the original file. Disconnecting an integration does not delete the underlying agent account or its own files. Uninstalling may leave exported files or other local data behind; do not assume it erases every copy. Contact support for guidance on locating app data before deleting it.

## Network requests and third parties

Smart Notch is not entirely offline. Depending on the feature and version:

- **Microsoft Store** handles purchase, license checks, restoration and app distribution. The app receives product, price and entitlement information; it does not receive your payment-card details from Store checkout.
- **GitHub** hosts public update metadata, documentation and support. Update checks contact GitHub and may query Microsoft's Store listing services.
- **wttr.in** provides weather. A weather request exposes your network IP address to that service, which can use it to infer an approximate location.
- **LRCLIB** receives track/artist information and related lookup parameters to find lyrics.
- **Agent providers** receive requests required by the integration you connect. For example, Claude usage/profile queries use the signed-in account's authorization. Other integrations may communicate with a local Codex or Antigravity service or read a user-selected local usage report. The provider's own application may communicate with its servers.
- **Content and external actions:** remote artwork or custom backgrounds can contact their hosting services. Opening a website or a clipboard web-search action sends the selected URL or search text to the destination service.

Online services receive normal connection information, including your IP address and request metadata, and apply their own privacy policies. Examples include [Microsoft](https://privacy.microsoft.com/privacystatement), [GitHub](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement), and the relevant media, weather, search or agent provider.

The app does not implement an advertising tracker or a developer-operated upload service for clipboard history. This does not mean that no data leaves your device: the feature-specific requests above and any information you choose to submit to support are separate disclosures.

## Your choices

Use the available settings to manage visible widgets and notifications, disconnect integrations, and remove saved history items. A visibility setting is not necessarily a data-processing switch: in version 7.1.5, clipboard monitoring starts with the app, and the main interface requests weather on startup even when its weather widget is hidden. Removing the copied-link popup does not stop clipboard history capture. Some detected integrations can initialize automatically or reconnect from saved settings. Availability of individual controls varies by edition and version. Exit Smart Notch to stop its ongoing processing; clearing existing history does not prevent new items from being captured while the app remains running. You can also manage provider permissions and revoke credentials through the provider's own application or account settings.

To request help accessing or removing locally stored app information, contact support. We cannot remotely read or erase data that is stored only on your computer. Microsoft and other providers manage data stored in their own services.

## Support information

If you submit an issue, its text and attachments are public on GitHub. Share only the minimum information needed to explain the problem. Do not post passwords, access tokens, payment details, private clipboard contents or unreviewed logs. For a sensitive issue, first request a private contact method without including the sensitive information itself.

Support submissions are used to investigate and respond to the issue. GitHub hosts and retains them according to its settings and policies; closing an issue does not automatically delete it.

## Security and changes

The app relies on Windows account protections, the storage and authentication mechanisms of connected providers, and secure connections where supported. No device or service can guarantee absolute security. Keep Windows, Smart Notch and connected agents updated.

This page will be updated when data handling changes. Review the updated date and the policy for the version you use. This policy does not replace the independent policies of Microsoft or connected services.

## Contact

Publisher: **Dev_avinash / Avenger11764**.

For privacy questions or a request for a private contact channel, use [Smart Notch support](https://github.com/Avenger11764/Smart-notch/issues/new). Do not include personal or sensitive information in a public issue.
