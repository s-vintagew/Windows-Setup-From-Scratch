## Contents
- [Windows Setup From Scratch](#windows-setup-from-scratch)
  - [Getting Started](#getting-started)
  - [Windows ISO Download](#windows-iso-download)
  - [Windows Installation](#windows-installation)
  - [Installating Office 365](#installating-office-365)
  - [Activating Windows Product](#activating-windows-product)
  - [Package Manager for Windows](#package-manager-for-windows)
  - [Web Browser](#web-browser)
    - [How do we choose a browser?](#how-do-we-choose-a-browser)
    - [What is recommended?](#what-is-recommended)
    - [Recommended Extensions](#recommended-extensions)
  - [Video Player](#video-player)
    - [MPV](#mpv)
  - [Archive File Managers](#archive-file-managers)
  - [Visual C++ Redistributable](#visual-c-redistributable)
  - [Photo Viewer](#photo-viewer)
  - [Audio Player](#audio-player)
  - [World of Torrent](#world-of-torrent)
  - [Contributing](#contributing)
  - [License](#license)

# Windows Setup From Scratch
I have faced timeless instances where after installing windows, I have to sit and recall which softwares are the most essential once and we damn as well need in our daily lives. Starting from media player and image viewer to vcredist for games. There are tonnes of adwares and useless crappy softwares which just consumes your CPU and RAM, resulting in less productivity etc. Well, I have tried to jot them all down so that it helps everyone. 

This repo will contain
- Microsoft Windows and Offie Downloads
- Essential software to install
- System configuration steps
- Useful PowerShell commands
- Customization tips

and maybe more.

## Getting Started
1. Review the list of recommended software and install as needed.
2. Follow the configuration steps to optimize your system.
3. Use the provided scripts and commands to automate setup tasks.

## Windows ISO Download
In this step, all you gotta have is one simple PC [borrow from friend or whatever] and follow the steps.

- ISO file download - https://massgrave.dev/genuine-installation-media. <br> Remember windows comes in 2 editions, consumer and business. For "Windows Home" download the Consumer edition and for "Windows Pro, Workstation or Education" download the Business Edition ISO.
- Rufus for making it bootable - https://rufus.ie/en/. 

After this all you will need is a Pendrive probably 32GB and you are good to run rufus, select the ISO and you are good to start.

## Windows Installation
During installation, windows gives you options to install various versions:

- Windows Home
- Windows Pro
- Windows Education
- Windows Education N
- Windows Workstation
  For someone who have less resources such as 8GB RAM and HDD can use https://rentry.co/windows_for_retards as a guide to install windows without telemetry etc for lesser CPU load. 

## Installating Office 365
Download the img file from https://gravesoft.dev/office_c2r_links
[Recommended download: O365ProPlusRetail - Offline x32-x64]

## Activating Windows Product
Download the file from the github repo: aHR0cHM6Ly9naXRodWIuY29tL2FiYm9kaTE0MDYvS01TX1ZMX0FMTF9BSU8=
[Turn of the Windows Antivirus real time scanning before downloading and executing the cmd file.]

For instruction refer to the link https://rentry.co/windows_for_retards#activation

## Package Manager for Windows
Windows has two widely used package managers.
- Winget: Comes out of the box in Windows 10 and Windows 11.
- Chocolatey: Can be easily installed.

Installting Chocolatey: https://chocolatey.org/install
For Packages and other details: https://community.chocolatey.org/

## Web Browser
When it comes to web browser, people prefer chrome due to it's ease of access and much more features such as translation etc. Little do we know that Firefox and Other browsers do provide the same features.

Popular Browsers:
- Firefox
- Google Chrome
- Edge
- Safari
- Brave

Unpopular Browsers:
- Librewolf
- Thorium
- TOR

### How do we choose a browser?
Below are the parameters you can use to choose a browser.
- Privacy [Does not collect user data] https://privacytests.org/
- Ease of Access [Smoothness, UI, etc.]
- Security [Preventing website tracking]
- Regular Updates [Stable updates by the developers/companies]
- Thriving Community [getting easy solutions to bugs and problems in case of mishaps] 
- Resource Consumption [Less Processor and RAM Heavy]
- Extensions [support for open and wide community developing various extensions for varied usage]
- Browser Engines. [Firefox has it's own browser engine where edge, brave, chrome runs on chromium engine]

Browser Comparison: https://eylenburg.github.io/browser_comparison.htm

### What is recommended?
It is recommended to use [Firefox](https://www.mozilla.org/en-US/firefox/new/). You can also try [Librewolf](https://librewolf.net/) [Fork of Firefox and much more secure]. Firefox has a wide variety of Extensions to make your browsing experience smooth, ad-free, secure and many more.

### Recommended Extensions
- [Ublock Origin](https://ublockorigin.com/)
- [Sponsorblock](https://github.com/ajayyy/SponsorBlock)
- [Enhancer for Youtube](https://www.mrfdev.com/enhancer-for-youtube)
- [Buster](https://github.com/dessant/buster#readme): For Auto-solving Captcha
- [Search by Image](https://github.com/dessant/search-by-image#readme)
- [Dark Reader](https://darkreader.org/)
- [Tab Stash](https://josh-berry.github.io/tab-stash/)
- [Turbo Download Manager](https://webextension.org/listing/turbo-download-manager-v2.html)
- [Tampermonkey](https://www.tampermonkey.net/): Run own scripts in browser

## Video Player
It's very obvious that "Media Player" of windows is useless and does not even play all types of video/audio files. It's better to use some community preffered, open source/freeware media players
- VLC media player [Freeware]
- MPV [Open Source]
  
Now that we have our package manager ready, we can easily install them with single line commands.
- Installing VLC: `choco install vlc`
- Installing mpv: `choco install mpv`
[Recommended]
### MPV
It's an open source project that supports almost all formats and codecs. It's a customizable media player. You can use lua scripting to change and modify the GUI as you wish.

- MPV Frontends: https://github.com/mpv-player/mpv/wiki/Applications-using-mpv
- UOSC: https://github.com/tomasklaen/uosc

There may be other media players out there but these are the most used and community friendly.

## Archive File Managers
Most common thing found in the internet, archives [zip/rar]. Most used tools: 
- winrar: Propreitary/Freeware, not recommended
- 7zip: Open Source, highly recommended

Installing 7zip: `choco install 7zip`

## Visual C++ Redistributable
Let's say you want to do graphics related stuff. Apart from the graphics driver you would also need visual c++ librarier and DirectX.

Installing vcredist: `choco install vcredist-all`
<br>
Installing directX: `choco install directx`

## Photo Viewer
Once again, let's not use the crappy windows photo viewer. There are much better and lightwright options available.

1. JPEGView - `choco install jpegview`
2. Faststone - `choco install fsviewer`

[JPEGView is recommended for simple viewing and simple photo based tasks]


## Audio Player
It is already expected that you will have spotify or youtube for this purpose. Nonetheless if you have downloaded songs and offline playlists, the players mentioned in [Video Player](#video-player) should do the trick.

There are dedicated players available too for audio playback.
1. MusicBee: `choco install musicbee`
2. Foobar: `choco install foobar2000`
   
Try and use both and keep the one that suits your UI preferences and accessibility.

## World of Torrent
This part is a pretty deep rabbit hole, the end of which is not known. With too many branches in the borrow, it's actually difficult to get started and to know, what's safe and how to be safe while torrenting.

Let's start from the basics:
1. You will need to follow the recommended browser options mentioned in [What is recommended?](#what-is-recommended) along with the Ad-Blocker extension [UBlock Origin].
2. Once that is setup you would need something called a torrent client. This client pulls files from the P2P network [basically a mesh of computers who have a files and are uploading them in parts]. <br> 
   - Qbittorrent: `choco install qbittorrent` [recommended, easy to use]
   - Transmission: `choco install transmission` <br>
  
    **Dont's:**
     - Do not Install utorrent or bittorrent. Those were reported to be running crypto mining scripts and flagged as malware.

3. Knowing about torrent tracker sites: These sites, list torrents and gives you a tracker file that your client understands. List of well knows torrent tracker sites: https://torrentfreak.com/top-torrent-sites/
4. How do you search for a torrent file:
   1. Head over to any tracker site. Example 1337x.to, now search for the file you need, let's say the movie 'How to Train Your Dragon'.
   2. Once you hit enter, there will be a list of trackers. Now select the one with the quality you need, size you can download and it's seeder:leecher ratio should be >1.
   3. Now once selected, click that tracker. Once in the next page look for a 'magnet link' or magent symbol and you should be redirected to qbittorrent.
   4. Start the download and you are already torrenting.
5. Use the specific sites mentioned in Point 3. There are lot many fake/mirror sites out there which are not official.


## Contributing
Feel free to submit pull requests or open issues to suggest improvements or add new setup tips.

## License
This project is licensed under the MIT License.

README file under construction 🚧