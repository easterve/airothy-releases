# airothy-releases

Public distribution channel for **AirothyServer** — the macOS half of [Airothy](https://github.com/easterve), an iOS ↔ macOS remote control system that turns your iPhone into a wireless trackpad and keyboard for your Mac.

## Download

The latest stable build of `AirothyServer.app` is always available on the [Releases page](https://github.com/easterve/airothy-releases/releases/latest).

Pre-release / beta builds are tagged with `-beta.N` and marked as pre-releases.

## System requirements

- macOS 15 or later
- Mac on the same local network as your iPhone
- Accessibility permission granted to AirothyServer in **System Settings → Privacy & Security → Accessibility**

## Auto-updates

Once installed, AirothyServer checks for updates automatically via [Sparkle](https://sparkle-project.org). The feed lives at [`appcast.xml`](./appcast.xml) in this repo. Opt in to beta builds inside the app's **Settings → Updates** panel.

## Why is this repo separate from the source?

Sparkle clients download updates unauthenticated, so the binaries and appcast have to live in a public location. The Airothy source code is hosted in a private repository.

## What's in a release

Each release attaches one asset:

- `AirothyServer.dmg` — Developer ID-signed, notarized, stapled, Sparkle-signed.

Verify the signature manually with [Sparkle's `sign_update` tool](https://sparkle-project.org/documentation/) if you want.

## License & support

Visit the [Airothy organization](https://github.com/easterve) for issue reporting and contact.
