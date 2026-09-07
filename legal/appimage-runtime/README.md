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

These notices do not cover every runtime dependency. The executable contains
Squashfuse and LZMA symbols; their exact linked source/build provenance and
applicable notices remain under review. The AppImageKit root license explicitly
excludes dependencies with different terms. No complete corresponding-source
or reproducible-build claim is made. Historical AppImage runtime prefixes have
not yet been compared. Existing downloads and private application source are
unchanged; these third-party terms do not license Notner itself.
