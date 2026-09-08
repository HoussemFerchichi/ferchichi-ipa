# Ferchichi for iPhone — builds

Sideloadable, **unsigned** builds of [Ferchichi](https://github.com/HoussemFerchichi/ferchichi-phone)
— a Stremio front end for iOS with a VLC-backed player, so MKV, AC3, DTS and
HEVC all play in the app rather than being handed to something else.

This repository holds the binary only; the source lives in a private repo.

## Install

Direct link, for any sideloader that takes a URL:

```
https://raw.githubusercontent.com/HoussemFerchichi/ferchichi-ipa/main/Ferchichi.ipa
```

The app is unsigned on purpose — your sideloader signs it with your own Apple
ID as it installs. On a free account that lasts seven days before it needs
re-signing, which is Apple's limit rather than the app's.

## First run

It asks for the address of a machine running Stremio Service or the Stremio
desktop app, something like `http://10.0.0.30:11470`. A phone cannot seed a
torrent itself, so that is what makes torrent sources play — and it only works
while the phone is on the same network as that machine. If your stream addon
returns ordinary HTTPS links, as a debrid service does, you can skip it.
