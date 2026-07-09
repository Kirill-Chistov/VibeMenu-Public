# VibeMenu

**Native macOS menu-bar radar for Claude coding sessions, usage limits, thermal pressure, and sleep prevention.**

VibeMenu lives in your menu bar and gives you an at-a-glance "radar" of your Claude
coding activity — which sessions are running, how close you are to your usage limits,
how hard your Mac is working, and whether it will stay awake while Claude is busy.

**Current release: v0.2 beta**

---

## Download

➡️ **[VibeMenu-v0.2-macOS-arm64.zip](releases/v0.2/VibeMenu-v0.2-macOS-arm64.zip)**
&nbsp;·&nbsp; [SHA-256](releases/v0.2/VibeMenu-v0.2-macOS-arm64.zip.sha256)

Verify your download (optional):

```sh
shasum -a 256 -c VibeMenu-v0.2-macOS-arm64.zip.sha256
```

## Install

1. **Unzip** `VibeMenu-v0.2-macOS-arm64.zip`.
2. **Move** `VibeMenu.app` into your `/Applications` folder.
3. **Open** it. VibeMenu runs as a menu-bar app (no Dock icon) — look for its icon
   in the top-right of your screen.

## Requirements

- **macOS 15 (Sequoia) or later**
- **Apple Silicon**

## Security note

VibeMenu v0.2 beta is **not signed with an Apple Developer ID certificate and is not
notarized**. On first launch, macOS Gatekeeper may refuse to open it.

To open it anyway:

1. **Right-click** (or Control-click) `VibeMenu.app` → **Open**.
2. In the dialog that appears, click **Open** again.

You only need to do this once. (If you prefer, you can also allow it from
**System Settings → Privacy & Security** after the first blocked launch.)

## Privacy

VibeMenu is **local-only**:

- **No telemetry.** Nothing about your usage is collected or reported.
- **No network calls.** The app does not talk to any server or backend.
- **No backend, no accounts, no API keys.**

It reads only the local Claude-related files it needs to show session titles and, if
you enable it, usage-limit info. Everything stays on your Mac. See
[PRIVACY.md](PRIVACY.md) for details.

## Features

- **Claude Session Radar** — see your active Claude coding sessions at a glance.
- **Claude Usage Limits Preview** — know where you stand before you hit a wall.
- **5-hour / weekly / model-specific limit rows** — the limits that matter, broken out.
- **Per-limit visibility** — show or hide individual limit rows to keep the menu tidy.
- **Thermal pressure** — a heads-up when your Mac is running hot.
- **Sleep prevention** — keep your Mac awake while Claude is working.

## Source code

VibeMenu's **source code is private and proprietary.** This repository contains only
the public download, release notes, and documentation. The app binary is provided
under the license in [LICENSE.md](LICENSE.md); no source-code rights are granted.

## Support

Found a bug or have a request? If Issues are enabled on this repository, please open
one here. Include your macOS version and a clear description of what you saw versus
what you expected.

---

© 2026 Dmitrii / Kirill Chistov. All rights reserved. VibeMenu is not affiliated with
or endorsed by Anthropic. "Claude" is a trademark of Anthropic, PBC.
