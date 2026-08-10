<div align="center">

# 📥 fetchIT

**A Bash-based command-line media downloader for Ubuntu Linux**

Powered by the open-source [`yt-dlp`](https://github.com/yt-dlp/yt-dlp) engine — supporting video, audio, and playlist downloads from thousands of websites.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Platform](https://img.shields.io/badge/platform-Ubuntu%20Linux-orange)
![Shell](https://img.shields.io/badge/shell-Bash-4EAA25?logo=gnubash&logoColor=white)
![Status](https://img.shields.io/badge/status-active-brightgreen)

</div>

---

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Future Plans](#future-plans)
- [License](#license)

---

## Features

| | |
|---|---|
| 🎥 **Video Downloads** | Download videos in the best available quality and format |
| 🎵 **Audio Downloads** | Extract and download audio from supported media |
| 📋 **Playlist Downloads** | Download complete playlists with ease |
| 🌐 **Multi-Website Support** | Download media from thousands of websites supported by `yt-dlp` |
| 📜 **Download History** | Keep track of previously downloaded media |
| 📊 **Download Statistics** | View useful statistics about your downloads |
| 📁 **Download Management** | Organize downloaded videos, audios, and playlists into separate directories |
| ⚙️ **Dependency Management** | Check for required dependencies and assist with their installation |
| 💻 **Command-Line Interface** | Lightweight and fully terminal-based, with no graphical interface required |
| 🐧 **Ubuntu Linux Support** | Designed specifically for Ubuntu-based Linux environments |

---

## Requirements

| Requirement | Purpose |
|---|---|
| **Ubuntu Linux** | Target operating system |
| **Bash** | Shell used to run fetchIT |
| **[yt-dlp](https://github.com/yt-dlp/yt-dlp)** | Media downloading and extraction engine |
| **FFmpeg** | Audio/video processing |
| **Deno** | JavaScript runtime required by `yt-dlp` for certain sites and extraction features |
| **Internet Connection** | Required for downloading media and accessing supported websites |

> fetchIT checks for these dependencies on first run and will assist with installing any that are missing.

---

## Installation

**1. Clone the repository**

```bash
git clone git@github.com:rubayet-ashib/fetchIT.git
cd fetchIT
```

**2. Make the scripts executable**

```bash
chmod +x main.sh config.sh
```

**3. Run fetchIT**

```bash
./main.sh
```

On the first run, fetchIT will check for its required dependencies and create the necessary runtime files and directories automatically.

---

## Usage

After installation, start fetchIT from the project directory:

```bash
./main.sh
```

fetchIT provides an interactive command-line interface that guides you through the available download and management options.

From the main menu, you can access features such as:

- Video downloading
- Audio downloading
- Playlist downloading
- Inspecting video information
- Download history
- Download statistics

Follow the prompts displayed in the terminal to select an operation and provide the required media URL or options.

---

## Project Structure

```
fetchIT/
├── main.sh                 # Main entry point and application flow
├── config.sh               # Configuration and runtime setup
├── lib/
│   ├── downloader.sh       # Media downloading functionality
│   ├── history.sh          # Download history management
│   ├── manager.sh          # Download/file management
│   ├── stats.sh            # Download statistics
│   └── ui.sh               # Command-line interface and UI functions
├── downloads/               # Runtime directory for downloaded media
│   ├── videos/
│   ├── audios/
│   └── playlists/
├── history.csv              # Runtime download history
├── .gitignore                # Files and directories excluded from Git
├── LICENSE                    # MIT License
├── README.md                  # Project documentation
└── CHANGELOG.md               # Project version history
```

> **Note:** `history.csv` and the contents of `downloads/` are generated at runtime and are not included in the Git repository.

---

## Future Plans

- [ ] Windows version with an improved graphical user interface
- [ ] Additional platform support
- [ ] Further performance and usability improvements

---

## License

fetchIT is open-source software licensed under the [MIT License](LICENSE).

---

<div align="center">

Made with 🐧 for the command line

</div>
