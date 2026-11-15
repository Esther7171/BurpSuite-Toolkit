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

- **Windows:** Inline guide below
- **Ubuntu:** [View Installation Guide](https://github.com/Esther7171/BurpSuite-Toolkit/tree/main/doc/Setup-guide/Ubuntu)

### Windows

This guide walks you through installing Burp Suite on Windows 10 or Windows 11 using a simple, Java-based setup. Follow each step in order and you will have Burp Suite running in a few minutes.

#### Requirements

- Windows 10 or Windows 11 (64-bit)
- Java 21 or Java 25 (recommended for this setup)
- BurpLoader
- Burp Suite JAR file from the official PortSwigger website or from the project releases
#### 1. Install Java

Download Java 21 or Java 25 for Windows. Pick whichever version you prefer. Java 25 is already installed on my machine, so that is what this guide uses.

- [Download Java 21 (Windows x64)](https://download.oracle.com/java/21/archive/jdk-21.0.9_windows-x64_bin.msi)
- [Download Java 25 (Windows x64)](https://www.oracle.com/java/technologies/javase/jdk25-archive-downloads.html)

Open the downloaded `.msi` installer, follow the wizard, and complete the installation.

#### Verify Java Installation

Open PowerShell or Command Prompt and run:

```powershell
java -version
```

If Java is installed correctly, the command will display the installed Java version.

<details>
#### <summary><strong>1.1 Organize Your Files (For Beginners)</strong></summary>

Let's keep everything in one place before we download anything. I am using the Documents folder because I do not like a messy Desktop on Windows. You can choose any folder you like.

Create a folder called `burpsuite` inside Documents. I am using the terminal because it is quicker for me.

```powershell
PS C:\Users\<USERNAME>> cd .\Documents\
PS C:\Users\<USERNAME>\Documents> mkdir burpsuite
PS C:\Users\<USERNAME>\Documents> cd .\burpsuite\
PS C:\Users\<USERNAME>\Documents\burpsuite>
```

Now your terminal is inside the folder where we will download the JAR file.

</details>

---

#### 2. Download Burp Suite

You can download the Burp Suite JAR file from two places. Both options give you the same JAR format, so pick whichever is easier for you. The goal is to get a `.jar` file, not a Windows `.exe` installer.

<details>
<summary><strong>Quick download using the command line</strong></summary>

My terminal is already open in the same folder. If you prefer using the terminal, you can download the JAR file with `curl`. Open PowerShell or Command Prompt inside your `burpsuite` folder and run:

```powershell
curl "https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar" -o burpsuite_desktop_v2026.10.1.jar
```

This command saves the JAR file to your current folder. You can change the output name after `-o` if you want a different filename.

Be patient, the file is approximately `750 MB` in size.

##### Verify the download from the terminal

You can match the checksum to make sure the file downloaded correctly:

```powershell
Get-FileHash .\burpsuite_desktop_v2026.10.1.jar -Algorithm SHA256
```

If the hash matches the value below, you are good to go:

```
sha256:e8ab086537b1643b91ca09d2fc2a6c3e08a8bae0c85280797c5c9ec76506c3c5
```

</details>

<details>
<summary><strong>Option 1: Official download from PortSwigger</strong></summary>

[Download Burp Suite from PortSwigger](https://portswigger.net/burp/releases)

1. Open the download page.
2. Select the latest Professional or Community release.
3. Choose the standalone **JAR** format.
4. Save the `.jar` file to your Downloads folder.

</details>

<details>
<summary><strong>Option 2: Direct download from project releases</strong></summary>

If you want to skip the format selection and avoid any confusion, use the ready-made JAR files hosted on this project:

[Download Burp Suite JAR from Project Releases](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/Professional_and_Community)

Direct download link for the latest JAR:

[burpsuite_desktop_v2026.10.1.jar](https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar)

1. Open the release page or the direct link.
2. Download the `.jar` file.
3. Save it to your Downloads folder or any folder you prefer.

</details>

> **Important:** Choose the JAR format, not the Windows `.exe` installer, for this Java-based setup. The project release already provides the correct JAR format, so beginners can download it without worrying about picking the right file type.

---

#### 3. Download BurpLoader

BurpLoader is the small launcher that starts Burp Suite.

<details>
<summary><strong>Quick download using the command line</strong></summary>

If your terminal is still open inside the `burpsuite` folder, run:

```powershell
curl "https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar" -o burp-loader.jar
```

</details>

> **Option 1: [Download BurpLoader from the v1.0 Release page](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0)**  
> Look for `burp-loader.jar` in the assets list and save it to your `burpsuite` folder.

---

<details>
<summary><strong>3.1 Confirm Your Files Are in Place (For Beginners)</strong></summary>

Before we start setting things up, check that both files are in the same folder. Inside your `burpsuite` folder, run:

```powershell
ls
```

You should see both files listed:

```powershell
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        15-11-2026  07:07 PM        1238721 burp-loader.jar
-a----        15-11-2026  06:52 PM      751385742 burpsuite_desktop_v2026.10.1.jar
```

If both files are downloaded, you are all set. Now we can start setting it up.

</details>


#### 4. Launch BurpLoader

Navigate to the folder where BurpLoader is located and run the command below, or simply double click the `burp-loader.jar` file to launch it.

```powershell
java -jar burp-loader.jar
```

BurpLoader will open. Wait a moment. If both Burp Suite and BurpLoader are in the same folder, BurpLoader will locate Burp Suite on its own and show a `ready to start` message. You can then hit **Run** directly.

<img width="1287" height="583" alt="ready to start" src="https://github.com/user-attachments/assets/e0d611cf-fa0f-44b2-b216-82cb224858be" />

<details>
<summary><strong>If Burp Suite is in a different directory, or BurpLoader did not recognize it automatically</strong></summary>

If you installed BurpLoader and Burp Suite in different folders, or BurpLoader was not able to detect it even in the same location, use the **Browse** button to locate the Burp Suite JAR file manually.

<img width="1283" height="582" alt="browse for burpsuite jar" src="https://github.com/user-attachments/assets/2be23875-c670-4188-96bf-2297320f99df" />

Once you select the Burp Suite JAR with Browse, BurpLoader will show that Burp Suite was selected successfully. Hit **Run** and let's go.

<img width="1287" height="584" alt="burpsuite selected successfully" src="https://github.com/user-attachments/assets/5b00a8d6-7ba0-4d23-9d38-4152815950f7" />

</details>

When you press **Run**, be patient. The first launch of Burp Suite can take about 30 seconds to open, so do not spam the Run button.

When Burp Suite launches, it will ask you to continue with Professional or Community. Let's continue with Professional.

<img width="626" height="860" alt="choose professional or community" src="https://github.com/user-attachments/assets/862ad6ac-616f-41de-bf27-8322964a887e" />
