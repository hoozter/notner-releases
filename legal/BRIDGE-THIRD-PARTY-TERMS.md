# Third-party terms for notner Bridge

These terms apply to the Linux AppImages v1.0.0–v1.0.3 and take precedence
over any conflicting Notner restriction for the third-party components below.

Third-party components remain under their own licenses. Notner's proprietary
terms do not restrict the rights those licenses grant.

For the work combined with the LGPL libraries, you may modify the work for
your own use and reverse engineer it to debug those modifications, as required
by LGPL version 2 section 6 or LGPL version 2.1 section 6, as applicable. This
includes replacing the LGPL shared libraries with modified, interface-compatible
versions. No conflicting Notner restriction or termination term limits these
permissions. This exception does not make Notner open source or grant rights
to redistribute its proprietary application code.

The [library notices and corresponding source packages](README.md#ubuntu-source-packages)
are supplied alongside these terms.

## Replacing a shared library

Work on a copy in a directory you own; keep the original download unchanged.
Extract the AppImage's filesystem with its `--appimage-extract` option, or with
an AppImage-aware SquashFS extraction tool. In the resulting `squashfs-root`,
replace the relevant file in `usr/lib` with your modified, interface-compatible
library, preserving its expected shared-library name. Launch `./AppRun` from
that extracted directory, rather than launching the original AppImage.

The inspected launcher puts the extracted `usr/lib` first in
`LD_LIBRARY_PATH`. This is a shared-library replacement route; rebuilding or
publishing Notner's private source is not required for that operation. A
replacement must preserve the library's ABI and satisfy its dependencies.
The launcher and library layout were inspected; arbitrary modified libraries
have not been runtime-tested.
