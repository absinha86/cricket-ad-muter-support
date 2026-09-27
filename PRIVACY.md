# Privacy Policy: Cricket Ad Muter

_Last updated: 27 September 2026_

Cricket Ad Muter is a browser extension that mutes, or turns down, ad breaks during live cricket on JioHotstar. It is built to work entirely inside your browser.

## What the extension does not do

- It does **not** collect, sell, or share any personal information.
- It does **not** send your browsing history, the pages you visit, or anything about what you watch to the developer or to anyone else.
- It has **no** analytics, tracking, advertising, or accounts.
- It does **not** block, change, or skip ads, and it does not alter any network request.

## What stays on your device

The extension stores the following **only in your browser** (Chrome's extension storage). None of it is ever transmitted:

- Your settings, such as mute or lower volume, alert preferences, and timing options. If you use Chrome Sync, Chrome may sync these settings between your own devices.
- A list of the last 200 ads it muted (the ad's name as JioHotstar labels it, its length, and the time). This powers the "Recent ads" list and the daily totals. You can clear it at any time with **Advanced → Reset stats**.

## How ad detection works

When an ad starts, the JioHotstar page sends a tracking request to JioHotstar's own servers. The extension watches for that request, **on JioHotstar domains only**, to know an ad has begun and how long it runs. It reads the request without blocking or modifying it, and it doesn't store or send it anywhere, apart from the ad name kept in the local list above.

## Network requests the extension makes

About every 6 hours, the extension downloads a small public file (`rules.json`) from the project's GitHub repository (`github.com/absinha86/cricket-ad-muter-support`). This file holds the patterns used to recognise ads, so detection can be fixed quickly if JioHotstar changes something. The request carries no information about you beyond what any web request includes, such as your IP address, which GitHub receives under its own privacy policy. The file contains data only, not code.

## "Report a problem"

If you choose **Report a problem**, the extension opens a pre-filled GitHub issue page. It includes the extension version, the rules version, your Chrome version, your mode setting, and the names of the last few ads detected. Nothing is sent until you review it and submit it yourself on GitHub.

## Permissions and why they are needed

| Permission | Why |
|---|---|
| Access to `hotstar.com` / `jiohotstar.com` (optional, you grant it) | To notice when an ad starts, and to time the ad break on the match page. The extension asks for this after install, and you can remove it any time in Chrome's extension settings. It never has access to any other site. |
| `webRequest` | To see (not block or change) JioHotstar's ad-start request |
| `storage` | To save your settings and the local list of muted ads |
| `notifications` | For the optional "The match is back" alert |
| `scripting` | To load the extension's own script on JioHotstar pages once you grant access, including tabs that were already open |
| `alarms` | To check for updated detection rules every few hours |

## Contact

Questions or concerns: open an issue at <https://github.com/absinha86/cricket-ad-muter-support/issues>.

Cricket Ad Muter is an independent project and is not affiliated with, endorsed by, or sponsored by JioStar, JioHotstar, or any cricket board.
