## Contents
- [Windows Setup From Scratch](#windows-setup-from-scratch)
  - [Getting Started](#getting-started)
  - [Windows ISO Download](#windows-iso-download)
  - [Windows Installation](#windows-installation)
  - [Installating Office 365](#installating-office-365)
  - [Activating Windows Product](#activating-windows-product)
  - [Package Manager for Windows](#package-manager-for-windows)
  - [Media Player](#media-player)
    - [MPV](#mpv)
  - [Archive File Managers](#archive-file-managers)
  - [Web Browser](#web-browser)
    - [How do we choose a browser?](#how-do-we-choose-a-browser)
  - [Contributing](#contributing)
  - [License](#license)

# Windows Setup From Scratch
I have faced timeless instances where after installing windows, I have to sit and recall which softwares are the most essential once and we damn as well need in our daily lives. Starting from media player and image viewer to vcredist for games. Well, I have tried to jot them all down so that it helps everyone. 

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

## Media Player
It's very obvious that "Media Player" of windows is process heavy and does not even play all types of video/audio files.
- VLC media player
- MPV
Now that we have our package manager ready, we can easily install them with single line commands.
- Installing VLC: `choco install vlc`
- Installing mpv: `choco install mpv`
[Recommended MPV]
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

## Web Browser
When it comes to web browser, people prefer chrome due to it's ease of access and much more features such as translation etc. Little do we know that Firefox and Other browsers do provide the same features.

Popular Browsers:
- Firefox
- Google Chrome
- Edge
- Safari
- Brave

Unpopular Browsers:
- Librefox
- Thorium
- TOR

### How do we choose a browser?
Below are the parameters you can use to choose a browser.
- Privacy [Does not collect user data]
- Ease of Access [Smoothness, UI, etc.]
- Security [Preventing website tracking]
- Regular Updates [Stable updates by the developers/companies]
- Thriving Community [getting easy solutions to bugs and problems in case of mishaps]
- Resource Consumption [Less Processor Heavy]
- Extensions [open and wide community developing various extensions for varied usage]

## Contributing
Feel free to submit pull requests or open issues to suggest improvements or add new setup tips.

## License
This project is licensed under the MIT License.

README file under construction 🚧