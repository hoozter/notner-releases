# notner releases

Official downloadable releases for notner companion applications.

## notner Bridge for Linux

The notner Bridge companion connects a signed-in Codex CLI to notner. It can
serve the browser directly on the same computer or maintain an outbound
connection to the notner-owned remote relay. It also provides Start, Stop,
Restart, and Quit controls through its window and Linux system tray.

[Download the latest Linux x86_64 AppImage](https://github.com/hoozter/notner-releases/releases/latest/download/notner-bridge-linux-x86_64.AppImage)

Requirements:

- Linux x86_64
- Codex CLI installed and signed in

After downloading:

```bash
chmod +x notner-bridge-linux-x86_64.AppImage
./notner-bridge-linux-x86_64.AppImage
```

Release checksums are included in each release description. This repository
contains release artifacts only; deployment and self-hosting documentation is
maintained with the notner source.
