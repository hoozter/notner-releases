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

## Linux helper libraries — v1.0.0–v1.0.3

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

All six library hashes also match in v1.0.0, v1.0.1, and v1.0.2. Each
historical AppImage was checked against its published whole-file SHA-256;
no artifacts have been replaced.

### Ubuntu source packages

The [source-package index](linux-source-packages.json) records the original
binary packages, source-package descriptions (`.dsc`), upstream source
archives, and Debian packaging archives or patches. All twelve source
archives/patches were downloaded and their sizes and SHA-256 hashes matched
the corresponding `.dsc` metadata. These include the upstream source and
Ubuntu/Debian packaging materials for the six helper-library packages.
OpenPGP signatures were not independently validated.

This index provides verified source locations, not a promise that external
archives will remain available or a complete corresponding-source delivery.
Reproducible builds and any additional conveyance obligations have not been
established. The application’s native helper and the AppImage runtime remain
under review; these notices do not establish complete compliance.

## Native Rust helper — supplemental crate notices

The retained `notner-safe-files` executable matches the helper in all four
AppImages (SHA-256 `1edc7c21c49b61ec9a41cc2d8384298d2c44c0410ae17a7e568e6b4043f78a03`). Its retained Cargo
lockfile and dependency files identify the crate versions indexed below.
All crate archives were checked against their lockfile SHA-256 checksums.

[Crate index and original legal files](rust-helper/index.json) includes the
entire retained dependency graph, including build-time procedural macros;
it does not assert that each crate is linked into the shipped executable.
The original license files are unmodified. No private application source
is included, and these texts do not license Notner itself.

This supplement is not a reproducible-build attestation or complete binary
bill of materials. Existing downloads are unchanged.

### Rust standard library

The helper records rustc revision `4a4ef493e3a1488c6e321570238084b38948f6db`
(Rust 1.94.0). The installed toolchain reports that same revision.
Its unmodified [standard-library copyright notices](rust-runtime/COPYRIGHT-library.html)
are supplied with the original [MIT](rust-runtime/LICENSE-MIT) and
[Apache 2.0](rust-runtime/LICENSE-APACHE) texts from that Rust revision.
The upstream notice includes other targets and build dependencies; their
inclusion does not mean they are linked into this Linux executable.

The same Rust revision supplies the original
[compiler-builtins terms](rust-runtime/compiler-builtins-LICENSE.txt), including
the LLVM exception, and its referenced [libm notices](rust-runtime/libm-LICENSE.txt).
The referenced [compiler-rt contributor list](rust-runtime/compiler-rt-CREDITS.TXT)
is also included. These are upstream notices, not an inventory of linked routines.

AppImage v1.0.0–v1.0.3 have identical runtime prefixes, with [verified upstream
provenance and supplemental original notices](appimage-runtime/README.md).
Runtime dependency coverage and the source-delivery limitations above remain
unresolved.
