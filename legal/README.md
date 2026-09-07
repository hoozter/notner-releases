# Supplemental third-party notices: notner Bridge v1.0.0–v1.0.3

The Linux x86_64 AppImages for these existing releases contain postgres 3.4.9
and saxes 6.0.0 in resources/app.asar. Their npm files were compared across all
four published artifacts. The following upstream notices supplement the
notices already included in those downloads:

- [postgres 3.4.9 — Unlicense](npm-postgres-3.4.9-LICENSE)
- [saxes 6.0.0 — ISC and retained sax notice](npm-saxes-6.0.0-LICENSE)

Original sources:

- https://github.com/porsager/postgres/blob/v3.4.9/UNLICENSE
- https://github.com/lddubeau/saxes/blob/v6.0.0/LICENSE

These are unmodified third-party legal texts, not a license grant for Notner.
They are supplemental notices, not a claim that every native-library or
corresponding-source obligation has been resolved. Existing AppImage bytes
and release checksums are unchanged.

## Linux helper libraries — v1.0.3

The six shared libraries below were matched byte-for-byte to their original
Ubuntu binary packages. These are the unmodified copyright files from those
packages, including their file-specific license terms.

- `libgconf-2.so.4`: [linux-libgconf-2.so.4-copyright](linux-libgconf-2.so.4-copyright) — [original Ubuntu package](https://archive.ubuntu.com/ubuntu/pool/main/g/gconf/libgconf-2-4_3.2.6-0ubuntu2_amd64.deb).
- `libnotify.so.4`: [linux-libnotify.so.4-copyright](linux-libnotify.so.4-copyright) — [original Ubuntu package](https://old-releases.ubuntu.com/ubuntu/pool/main/libn/libnotify/libnotify4_0.7.6-1ubuntu3_amd64.deb).
- `libappindicator.so.1`: [linux-libappindicator.so.1-copyright](linux-libappindicator.so.1-copyright) — [original Ubuntu package](https://old-releases.ubuntu.com/ubuntu/pool/main/liba/libappindicator/libappindicator1_12.10.1+13.10.20130920-0ubuntu4_amd64.deb).
- `libindicator.so.7`: [linux-libindicator.so.7-copyright](linux-libindicator.so.7-copyright) — [original Ubuntu package](https://archive.ubuntu.com/ubuntu/pool/main/libi/libindicator/libindicator7_12.10.2+14.04.20140402-0ubuntu1_amd64.deb).
- `libXtst.so.6`: [linux-libXtst.so.6-copyright](linux-libXtst.so.6-copyright) — [original Ubuntu package](https://old-releases.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst6_1.2.2-1_amd64.deb).
- `libXss.so.1`: [linux-libXss.so.1-copyright](linux-libXss.so.1-copyright) — [original Ubuntu package](https://old-releases.ubuntu.com/ubuntu/pool/main/libx/libxss/libxss1_1.2.2-1_amd64.deb).

Full license texts referenced by these notices: [LGPL-2](LGPL-2),
[LGPL-2.1](LGPL-2.1), and [GPL-3](GPL-3).

The libraries also match the immutable [appimage-12.0.1 upstream tree](https://github.com/electron-userland/electron-builder-binaries/tree/57839c6516289c0412c1b0887a6718d71e1ac5c2/AppImage/lib/x64).
The [upstream packaging script](https://github.com/electron-userland/electron-builder-binaries/blob/57839c6516289c0412c1b0887a6718d71e1ac5c2/appImage-packages-x64.sh) identifies the original Ubuntu packages.

This native-library comparison covers v1.0.3 only. Corresponding source and
build materials, the application’s native helper, and the AppImage runtime
remain under review; these notices do not establish complete compliance.
