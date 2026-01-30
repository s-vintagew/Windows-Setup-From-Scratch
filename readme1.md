# Windows Setup From Scratch

I have faced timeless instances where after installing Windows, I have to sit and recall which software is the most essential and what we damn well need in our daily lives. Starting from media players and image viewers to vcredist for games. There are tons of adware and useless crappy software that just consume your CPU and RAM, resulting in less productivity.

I have tried to jot them all down to help everyone.

**This repo contains:**
- Microsoft Windows and Office Downloads
- Essential software to install
- System configuration steps
- Useful PowerShell commands
- Customization tips

## Contents
- [Windows Setup From Scratch](#windows-setup-from-scratch)
  - [Contents](#contents)
  - [Getting Started](#getting-started)
  - [Windows ISO Download](#windows-iso-download)
  - [Windows Installation](#windows-installation)
  - [Installing Office 365](#installing-office-365)
  - [Activating Windows Product](#activating-windows-product)
  - [Package Manager for Windows](#package-manager-for-windows)
  - [Web Browser](#web-browser)
    - [How do we choose a browser?](#how-do-we-choose-a-browser)
    - [What is recommended?](#what-is-recommended)
    - [Recommended Extensions](#recommended-extensions)
  - [Media Player \& Tools](#media-player--tools)
    - [The Ultimate Downloader: yt-dlp](#the-ultimate-downloader-yt-dlp)
  - [Archive File Managers](#archive-file-managers)
  - [Visual C++ Redistributable](#visual-c-redistributable)
  - [Photo Viewer](#photo-viewer)
  - [Audio Player](#audio-player)
  - [World of Torrent](#world-of-torrent)
    - [The Setup](#the-setup)
    - [⚠️ CRITICAL SAFETY: Bind Your VPN](#️-critical-safety-bind-your-vpn)
    - [How to Search](#how-to-search)
  - [Antivirus](#antivirus)
  - [Contributing](#contributing)
  - [License](#license)

## Getting Started
1. Review the list of recommended software and install as needed.
2. Follow the configuration steps to optimize your system.
3. Use the provided scripts and commands to automate setup tasks.

## Windows ISO Download
In this step, all you need is a simple PC (borrow from a friend if needed) and follow the steps.

- **ISO file download:** [Massgrave - Genuine Installation Media](https://massgrave.dev/genuine-installation-media)
  - *Note:* Windows comes in 2 editions: Consumer and Business.
  - For "Windows Home", download the **Consumer Edition**.
  - For "Windows Pro, Workstation, or Education", download the **Business Edition**.
- **Bootable USB Tool:** [Rufus](https://rufus.ie/en/)

After downloading, you will need a Pen drive (probably 32GB). Run Rufus, select the ISO, and you are good to start.

## Windows Installation
During installation, Windows gives you options to install various versions:
- Windows Home
- Windows Pro
- Windows Education / Education N
- Windows Workstation

> **Tip:** For hardware with limited resources (e.g., 8GB RAM, HDD), you can use [this guide](https://rentry.co/windows_for_retards) to install Windows without telemetry for lower CPU load.

## Installing Office 365
Download the img file from [Gravesoft](https://gravesoft.dev/office_c2r_links).
* **Recommended download:** `O365ProPlusRetail - Offline x32-x64`

## Activating Windows Product
Download the file from the GitHub repo: `aHR0cHM6Ly9naXRodWIuY29tL2FiYm9kaTE0MDYvS01TX1ZMX0FMTF9BSU8=` (Decode Base64)

> **⚠️ Important:** Turn off Windows Antivirus real-time scanning before downloading and executing the cmd file.

For instructions, refer to: [Activation Guide](https://rentry.co/windows_for_retards#activation)

## Package Manager for Windows
Windows has two widely used package managers, plus a community favorite for power users.

- **Winget:** Comes out of the box in Windows 10 and 11.
- **Chocolatey:** Reliable and widely used.
- **Scoop:** Installs apps in your user folder (no UAC prompts) and avoids PATH pollution. Great for command-line tools.

**Installing Chocolatey:**
Visit [chocolatey.org/install](https://chocolatey.org/install)

**Installing Scoop (PowerShell):**
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

## Web Browser
When it comes to web browsers, people often default to Chrome. However, Firefox and other browsers provide better privacy and equal features.

**Popular Browsers:**
- Firefox
- Google Chrome
- Edge
- Brave

**Privacy-Focused / Niche Browsers:**
- **Librewolf** (Hardened Firefox fork)
- **Ungoogled Chromium** (Chrome without the Google tracking)
- **Thorium** (Performance optimized)
- **Tor**

### How do we choose a browser?
Below are the parameters you can use to choose a browser:
- **Privacy:** Does not collect user data. (Test at [PrivacyTests.org](https://privacytests.org/))
- **Security:** Preventing website tracking and fingerprinting.
- **Updates:** Regular, stable updates by developers.
- **Community:** Getting easy solutions to bugs.
- **Resource Consumption:** RAM and CPU efficiency.
- **Extensions:** Support for a wide variety of plugins.
- **Engine:** Gecko (Firefox) vs. Blink (Chromium).

**Browser Comparison:** [See Comparison Table](https://eylenburg.github.io/browser_comparison.htm)

### What is recommended?
It is recommended to use [Firefox](https://www.mozilla.org/en-US/firefox/new/) or [Librewolf](https://librewolf.net/) (a fork of Firefox that is much more secure). Firefox has a wide variety of extensions to make your browsing experience smooth, ad-free, and secure.

### Recommended Extensions
- [uBlock Origin](https://ublockorigin.com/) (Essential)
- [SponsorBlock](https://github.com/ajayyy/SponsorBlock)
- [Enhancer for Youtube](https://www.mrfdev.com/enhancer-for-youtube)
- [Buster](https://github.com/dessant/buster#readme): Auto-solving Captchas.
- [Search by Image](https://github.com/dessant/search-by-image#readme)
- [FastForward](https://fastforward.team/): Bypasses link shorteners.
- [Dark Reader](https://darkreader.org/)
- [Tab Stash](https://josh-berry.github.io/tab-stash/)
- [Turbo Download Manager](https://webextension.org/listing/turbo-download-manager-v2.html)
- [Tampermonkey](https://www.tampermonkey.net/): Run userscripts.

## Media Player & Tools
The default Windows Media Player is limited. Use community-preferred, open-source alternatives.

- **VLC Media Player** (Classic, reliable)
- **MPV** (Lightweight, highly customizable, best playback quality)

**Installation via Chocolatey:**
```powershell
choco install vlc
choco install mpv
```

**MPV & MPV.net**

MPV is powerful but lacks a GUI menu by default.
- **[mpv.net](https://github.com/mpvnet-player/mpv.net):** A modern frontend for MPV that adds a right-click menu and settings dialog, making it feel like a native Windows app.
- **[UOSC](https://github.com/tomasklaen/uosc):** A minimalist UI script for vanilla MPV.

### The Ultimate Downloader: yt-dlp
For downloading videos/audio from YouTube, Twitch, and thousands of other sites, **yt-dlp** is the gold standard.
- **Install:** `choco install yt-dlp` or `scoop install yt-dlp`
- **Note:** You also need **FFmpeg** for it to merge the best quality video and audio streams.
  - Install command: `choco install ffmpeg`
- **Usage:** `yt-dlp "LINK"`

## Archive File Managers
- **WinRAR:** Proprietary (Nagware).
- **7-Zip:** Open Source, highly recommended.
- **NanaZip:** A modern fork of 7-Zip for Windows 11 context menus.

**Install:** `choco install 7zip`

## Visual C++ Redistributable
Essential for gaming and graphics work.

- **All-in-One Installer:** `choco install vcredist-all`
- **DirectX:** `choco install directx`

## Photo Viewer
Replace the slow Windows Photos app with lightweight options.

1. **JPEGView:** Minimalist and fast. `choco install jpegview`
2. **FastStone Image Viewer:** Feature-rich. `choco install fsviewer`

## Audio Player
1. **MusicBee:** Great for managing large libraries. `choco install musicbee`
2. **Foobar2000:** Highly modular. `choco install foobar2000`


## World of Torrent
This is a deep rabbit hole. To stay safe, follow these rules.

### The Setup
1. **Browser + AdBlocker:** Ensure you are using Firefox + uBlock Origin.
2. **Torrent Client:**
   - **qBittorrent:** Open source, clean, no ads. (`choco install qbittorrent`)
   - **Transmission:** Simple and effective. (`choco install transmission`)
   - ❌ **Avoid:** uTorrent or BitTorrent (History of adware/miners).

### ⚠️ CRITICAL SAFETY: Bind Your VPN
If you use a VPN, you **must** bind qBittorrent to the VPN interface.
1. Open qBittorrent > **Tools** > **Options** > **Advanced**.
2. Look for **"Network Interface"**.
3. Change it from "Any interface" to your VPN adapter (e.g., `wg0`, `tun0`, or the name of your VPN driver).
4. **Why?** If your VPN disconnects, downloads stop instantly. No IP leaks.

### How to Search
1. Visit a trusted index (e.g., 1337x, TorrentGalaxy).
2. Search for your file (e.g., "Linux ISOs").
3. Check the **Seeder/Leecher ratio** (Should be > 1).
4. Click the **Magnet Link** (🧲) to open directly in your client.

## Antivirus
Common sense is the best antivirus. Windows Defender is usually sufficient for power users.

**Paid Options:**
- Kaspersky
- ESET NOD32
- Quick Heal

**Best Practices:**
1. Watch what you click. Check URLs.
2. Be careful with USB drives.
3. If suspicious, run a scan with **Malwarebytes** (Free version is a great second opinion scanner).

## Contributing
Feel free to submit pull requests or open issues to suggest improvements or add new setup tips.

## License
This project is licensed under the MIT License.

README file under construction 🚧