# AppImage runtime: verified provenance and supplemental notices

Scope: Notner v1.0.3 Linux x86_64 AppImage only. The retained full artifact
matches published SHA-256 `4bdbfbb2ca4915c2a4d3979ae5767b6f7cda883e5b86bc78b1a6173b86263077`.
Its first 188392 bytes match the electron-builder appimage-12.0.1
`runtime-x64` byte-for-byte, with SHA-256
`24da8e0e149b7211cbfb00a545189a1101cb18d1f27d4cfc1895837d2c30bc30`.
The runtime also matches Git blob `49a460f5420feb1bfe98f442f10058381b6bb644`
in [electron-builder-binaries at an immutable revision](https://github.com/electron-userland/electron-builder-binaries/blob/57839c6516289c0412c1b0887a6718d71e1ac5c2/AppImage/runtime-x64).

The embedded version string is `effcebc`, resolved to AppImageKit commit
`effcebc1d81c5e174a48b870cb420f490fb5fb4d`. This identifies the runtime's reported
source revision; it is not independent proof of a reproducible build.

- [Original AppImageKit license](LICENSE), from [upstream](https://raw.githubusercontent.com/AppImage/AppImageKit/effcebc1d81c5e174a48b870cb420f490fb5fb4d/LICENSE).
- [Original runtime.c copyright/permission header](runtime-source-notice.txt),
  preserved verbatim from [upstream](https://raw.githubusercontent.com/AppImage/AppImageKit/effcebc1d81c5e174a48b870cb420f490fb5fb4d/src/runtime.c), including Alexander Larsson's credit.
- [Reported source revision](https://github.com/AppImage/AppImageKit/tree/effcebc1d81c5e174a48b870cb420f490fb5fb4d).

## Squashfuse and liblzma

The reported AppImageKit revision pins libappimage to
`13f401a4a384ec59ec9a144e2a7006adf751571f`. Its
[dependency recipe](https://github.com/AppImage/libappimage/blob/13f401a4a384ec59ec9a144e2a7006adf751571f/cmake/dependencies.cmake)
selects Squashfuse `1f98030` and XZ Utils 5.2.3 by default. The runtime contains
Squashfuse and LZMA symbols. These recipe selections are not proof of the exact
linked source or build options.

- [Squashfuse license](squashfuse-LICENSE), preserved from revision
  [`1f980303b89c779eabfd0a0fdd36d6a7a311bf92`](https://github.com/vasi/squashfuse/tree/1f980303b89c779eabfd0a0fdd36d6a7a311bf92).
- [XZ Utils licensing notice](xz-COPYING), preserved from 5.2.3 revision
  [`3d566cd519017eee1a400e7961ff14058dfaf33c`](https://github.com/tukaani-project/xz/tree/3d566cd519017eee1a400e7961ff14058dfaf33c).
  It places liblzma source in the public domain. Its referenced
  [LGPLv2.1](xz-COPYING.LGPLv2.1), [GPLv2](xz-COPYING.GPLv2) and
  [GPLv3](xz-COPYING.GPLv3) texts are supplied for completeness of that notice;
  this does not mean the XZ command-line tools or build scripts are in Notner.

These supplements do not establish complete runtime dependency coverage or
corresponding-source delivery. Historical AppImage runtime prefixes have not
yet been compared. Existing downloads and private application source are
unchanged; these third-party terms do not license Notner itself.
