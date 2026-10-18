# Sonata releases

Signed releases and update feeds of **Sonata**, an unofficial Apple Music desktop app for Linux with
word-by-word lyrics. Not affiliated with Apple.

Project page: <https://github.com/MarcelineVPQ/apple-music-for-linux>

## What is here

| File | What it is |
|---|---|
| Releases → `sonata-X.Y.Z-x86_64.AppImage` | the app (development builds are marked *Pre-release*) |
| Releases → `sonata-X.Y.Z-source.tar.gz` | the complete source of that release (GPL-3.0) |
| Releases → `SHA256SUMS` | SHA-256 of every file in the release |
| `latest.json`, `latest-dev.json` (+ `.sig`) | the update feeds Sonata reads (Stable, Development), Ed25519-signed |

Sonata checks the feed's signature against the key built into the app, then the download's size and
SHA-512, before it installs anything. Never edit the feeds by hand: the release workflow writes and
signs them.

## Install

Download the newest `sonata-X.Y.Z-x86_64.AppImage` from Releases, then:

```bash
chmod +x sonata-*.AppImage
./sonata-*.AppImage
```

Sonata updates itself from here (Settings → Updates).

## Source and licence

Sonata is free software under the GNU General Public License v3.0. Each release carries its full
source as `sonata-X.Y.Z-source.tar.gz`; the licence text is `LICENSE` inside it.

## Bugs

Open an issue in this repository.
