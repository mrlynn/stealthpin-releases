# Stealthpin

Stealthpin changes where your iPhone appears in Find My, Maps and every other app. You run it from
your Mac, and the optional Stealthpin Remote app lets you drive it from the phone.

This repository only holds the built releases. The source code is private.

## What it does

- Set your iPhone's location anywhere on the map, or to a saved bookmark.
- Travel there instead of teleporting: drive, walk or cycle along real roads, taking as long as the
  real trip would.
- Natural GPS drift while the phone sits still, so the location doesn't look frozen.
- Replay trips you actually recorded, with their real stops and pace. GPX import and export.
- Back to Real Location from the window, the menu bar, ⇧⌘⌫ or the phone. Restarting the iPhone also
  switches faking off.
- Recents, suggested bookmarks and favorites.

## Requirements

- A Mac running macOS 14 or later.
- An iPhone with **Developer Mode** turned on (Settings › Privacy & Security › Developer Mode). The
  toggle appears after the phone has been connected to a Mac running Xcode at least once.
- [pymobiledevice3](https://github.com/doronz88/pymobiledevice3), which Stealthpin uses to talk to
  the phone:

  ```bash
  uv tool install pymobiledevice3
  ```

## Installing

1. Download the latest `Stealthpin.zip` from [Releases](../../releases).
2. Unzip it and move **Stealthpin** to Applications.
3. Connect your iPhone over USB, tap **Trust**, and open Stealthpin.
4. On iOS 17 and later, click the iPhone button at the top left of the map and choose **Start** to bring
   up the tunnel. It asks for your admin password, because the tunnel has to run as root.

If the macOS firewall is on, allow incoming connections for Stealthpin when asked, so the remote can
reach it.

Stealthpin Remote, the iPhone app, isn't offered as a download here, because iOS only installs apps
from the App Store, TestFlight or a developer's own build.

## Using it responsibly

Stealthpin is for controlling where your own iPhone appears. Faking a location can break the rules of
apps and services that depend on it, so use it with care.

Stealthpin isn't affiliated with or endorsed by Apple. Find My, iPhone and macOS are trademarks of
Apple Inc.
