<p align="center">
  <img src="Trialux-logo-on-navy.png" alt="Trialux: matter, trial and exhibit management" width="640">
</p>

# Trialux

**Matter, trial & exhibit management for Windows.** Trialux shows your exhibits to the jury on a second screen while you work from your own: highlight, call out, redact, stamp and point, without the jury ever seeing your menus, notes or the next exhibit.

This repository holds **official Trialux releases and update information only**. Trialux is commercial software; its source code is not published here.

## Download

Get the latest version from the [Releases page](../../releases/latest). Download **Trialux.exe**.

Trialux is a single portable program: there is nothing to install. Put `Trialux.exe` in a folder you can change, such as Documents or a USB drive, and run it. To let Trialux update itself, don't put it in Program Files.

## What it does

- **Present to the jury** on a second display or projector while you keep working on your own screen. Pause, freeze, side-by-side, call-outs and a laser pointer.
- **Mark up exhibits**: highlighting that snaps to the words, pen, arrows and shapes, redactions, and exhibit stamps in the usual sticker styles.
- **Organize a case**: exhibit numbers, groups, rulings (admitted or denied, with a warning before a denied exhibit reaches the jury), and search inside every exhibit, including scanned pages.
- **Documents, photos, audio and video** in one exhibit list.
- **Export**: marked PDFs, with redacted text removed for good and the rest kept searchable; a Word exhibit list; snapshots of what the jury saw.

## System requirements

- Windows 10 (version 2004 or later) or Windows 11, 64-bit
- A second display, projector or TV for presenting (optional for preparing)
- Internet access only for checking for updates; Trialux works fully offline

## Updates

Trialux checks this repository for a new version once a day, if allowed in Edit > Preferences, and tells you when one is available. To install it, choose **Help > Check for Updates**. Trialux downloads the new version, checks it and restarts. Nothing is installed without your say-so, and Trialux never updates while you are presenting.

Every release includes:

| File | What it is |
| --- | --- |
| `Trialux.exe` | The program |
| `manifest.json` | The version, download address and SHA-256 fingerprint of `Trialux.exe` |
| `manifest.json.sig` | A digital signature of `manifest.json` |

Trialux only accepts an update whose `manifest.json` is signed with the publisher's key, and whose download matches the fingerprint in that signed manifest.

### Checking a download yourself

In PowerShell, in the folder where you saved it:

```powershell
Get-FileHash .\Trialux.exe -Algorithm SHA256
```

The result should match the `sha256` value in that release's `manifest.json`.

## Support

Questions and problems: [SUPPORT CONTACT]

When reporting a problem, include your Trialux version (Help > About) and, if possible, the log file at `%LOCALAPPDATA%\Trialux\log.txt`.

## License

Copyright © 2026 JADTEB, LLC, an Iowa limited liability company. All rights reserved.

Trialux is licensed, not sold. Your use of it is governed by the license terms under which you received it. Nothing in this repository grants any right to copy, modify or distribute Trialux.

Trialux includes open-source components, each used under its own license. The full notices are in the program under **Help > Open-Source Licenses**. Those projects and their authors don't endorse Trialux.

Microsoft, Windows and Word are trademarks of the Microsoft group of companies.
