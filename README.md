# Cricket Ad Muter: support

This is the public home of **Cricket Ad Muter**, a Chrome extension that mutes, or turns down, ad breaks during live cricket on JioHotstar, and brings the sound back the moment play resumes.

## Found a problem?

[Open an issue](https://github.com/absinha86/cricket-ad-muter-support/issues/new). The quickest way is the **Report a problem** button in the extension's popup (under **Advanced**). It fills in the details that help, like the extension version and the last ads it detected, and you can review everything before submitting.

Helpful to include:
- what happened (an ad played with sound, or the match stayed muted, and for roughly how long)
- whether it was a live match or something else

## What's in this repo

| File | Purpose |
|---|---|
| [`rules.json`](rules.json) | Ad-detection patterns. The extension checks this file every few hours, so detection can be fixed without waiting for a store update. It contains data only, no code. |
| [`PRIVACY.md`](PRIVACY.md) | Privacy policy. In short: nothing is collected, and everything stays in your browser. |

---

Cricket Ad Muter is an independent project and is not affiliated with, endorsed by, or sponsored by JioStar or JioHotstar.
