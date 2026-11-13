<div align="center">

# BurpSuite 2026 Loader

<img width="180" alt="BurpSuite Toolkit Logo" src="https://github.com/user-attachments/assets/5f1e1607-96f1-4703-9589-21d07c4fecf1" />

**A lightweight, cross-platform Java utility for security research and authorized testing.**

![Latest](https://img.shields.io/badge/LATEST-v1.0-16a34a?style=plastic)
![Legacy](https://img.shields.io/badge/LEGACY-v0.9-ea580c?style=plastic)
![Platforms](https://img.shields.io/badge/PLATFORMS-Windows%20%7C%20Linux%20%7C%20macOS-2563eb?style=plastic)
![Documentation](https://img.shields.io/badge/DOCUMENTATION-Available-9333ea?style=plastic)

</div>

## Available Versions

| Version | Description | Release |
|---|---|---|
| **v1.0.0 (Latest)** | Automated edition with improved detection, GUI controls and shortcuts. | [Download v1.0.0](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0) |
| **v0.9 (Legacy)** | Original manual edition with the earlier interface and workflow. | [View v0.9 Release](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v0.9) |

## About the Project

BurpSuite 2026 Loader is a cross-platform, Java-based utility for **educational purposes, legitimate testing, and authorized security research**.

This repository provides loader information, compatibility details, installation instructions, and practical guides to help users get started.

## Features

- **Burp Suite Compatibility:** Designed for modern and legacy versions.
- **Lightweight:** Under 2 MB. No bulky installer.
- **Pure Java:** Single-JAR application.
- **Cross-Platform:** Windows, Linux and macOS. Testing is ongoing.
- **GUI-First:** Simple point-and-click interface.
- **Automatic JAR Detection:** Detects Burp Suite JAR files when available.
- **Manual JAR Selection:** Browse and select JAR files from other directories.
- **Desktop Shortcuts:** Create launchers for supported operating systems.
- **Built for Research:** Educational labs and authorized security testing.

## Tested Environments

| Operating System | Architecture | Status |
|---|---|---|
| Windows 10 | 64-bit | ✅ Tested |
| Windows 11 | 64-bit | ✅ Tested |
| Ubuntu | 64-bit | ✅ Tested |
| Kali Linux | 64-bit | ✅ Tested |
| Linux Mint | 64-bit | ✅ Tested |
| macOS | Apple Silicon (ARM64) | 🟡 Pending Testing |

**Java versions tested:** Java 21 and Java 25.

**Compatibility range:** Java 11–26 (not every version individually tested).

macOS testing is pending. Unfortunately, the Mac has left this world before testing could begin. 💀

## What's New in v1.0.0
### New Features
- **Java 11–26 Support:** Expanded Java runtime compatibility.
- **JAR Detection & Browse:** Automatically detects Burp Suite JAR files when available, or lets you manually browse and select one, whether it's in the same directory or somewhere else.
- **Download Options:** Quick access to official PortSwigger downloads and project-hosted releases, including Community and Professional JAR options.
- **Shortcut Creator:** Create desktop shortcuts and application launchers.

### UI & Experience
- Refreshed interface with a cleaner, responsive layout.
- Embedded application icons.
- **Copy & Paste Buttons:** Because doing things manually is overrated. A little less work, a little more laziness.

## Installation Guides

- **Ubuntu:** [View Installation Guide](https://github.com/Esther7171/BurpSuite-Toolkit/tree/main/doc/Setup-guide/Ubuntu)
- **Windows:** Installation guide coming soon. Expected by Sunday.

## FAQ

### 1. Which Java versions does BurpLoader support?

Tested with Java 11–25. For Burp Suite, Java 17 and Java 21 are currently recommended, with Java 21 preferred for stability. Future compatibility is not guaranteed.

### 2. Which Burp Suite format is supported?

Only the **Burp Suite `.jar` format** is supported across Windows, Linux and macOS. Installer packages such as `.exe`, `.deb`, and other OS-specific builds are not supported.

### 3. Why did you add download buttons?

After receiving requests through LinkedIn and GitHub issues, I added direct links to project releases and official PortSwigger downloads.

### 4. What's the difference between Community and Professional?

They are separate editions with different features and licensing. Check [PortSwigger's website](https://portswigger.net/burp) for details.

### 5. Does Burp AI work?

I haven't implemented or tested Burp AI integration. It may require signing in through the PortSwigger web portal. If you figure it out, feel free to teach me too! 😄

### 6. Can the legacy v0.9 run the latest Burp Suite?

Yes. The legacy v0.9 has been tested with Java 17 and Java 21. You can use Java 21 to run v0.9 alongside newer Burp Suite releases.

However, v0.9 is not compatible with Java 26 in my testing. For the best compatibility, use Java 21.

## Disclaimer

This project is provided for educational purposes and authorized security research.

- Use Burp Suite only on systems and applications you own or have explicit permission to test.
- Follow PortSwigger's official licensing terms and software usage policies.
- This project is not affiliated with, endorsed by, or sponsored by PortSwigger.
- The author is not responsible for misuse, unauthorized testing, or damages resulting from the use of this project.

**Use responsibly. Always obtain permission before testing.**

<div align="center">
  <img
    width="200"
    alt="Evil raccoon mascot"
    src="https://github.com/user-attachments/assets/346f7183-3440-4815-abe0-dcbd3072864c"
  />

  <p>Built and tested on my own machine. Yours might have a different opinion. 💀</p>

  <p>Something not working? Don't blame your keyboard just yet. Open an issue or find me on LinkedIn. We'll blame the bug together. 🤝</p>

  <p>If you found it useful, drop a ⭐. Feed the raccoon some motivation. 🦝</p>

</div>

