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

# Windows Installation Guide

This guide walks you through installing Burp Suite on Windows 10 or Windows 11 using a simple, Java-based setup. Follow each step in order and you will have Burp Suite running in a few minutes.

## Requirements

- Windows 10 or Windows 11 (64-bit)
- Java 21 or Java 25 (recommended for this setup)
- BurpLoader
- Burp Suite JAR file from the official PortSwigger website or from the project releases


## 1. Install Java

Download Java 21 or Java 25 for Windows. Pick whichever version you prefer. Java 25 is already installed on my machine, so that is what this guide uses.

- [Download Java 21 (Windows x64)](https://download.oracle.com/java/21/archive/jdk-21.0.9_windows-x64_bin.msi)
- [Download Java 25 (Windows x64)](https://www.oracle.com/java/technologies/javase/jdk25-archive-downloads.html)

Open the downloaded `.msi` installer, follow the wizard, and complete the installation.

### Verify Java Installation

Open PowerShell or Command Prompt and run:

```powershell
java -version
```

If Java is installed correctly, the command will display the installed Java version.

## 1.1 Organize Your Files (Recommended for Beginners)

Let's keep everything in one place before we download anything. I am using the Documents folder because I do not like a messy Desktop on Windows. You can choose any folder you like.

Create a folder called `burpsuite` inside Documents. I am using the terminal because that is what I prefer.

```powershell
PS C:\Users\<USERNAME>> cd .\Documents\
PS C:\Users\<USERNAME>\Documents> mkdir burpsuite

    Directory: C:\Users\<USERNAME>\Documents

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        15-11-2026  06:39 PM                burpsuite

PS C:\Users\<USERNAME>\Documents> cd .\burpsuite\
PS C:\Users\<USERNAME>\Documents\burpsuite>
```

Now your terminal is inside the folder where we will download the JAR file.

## 2. Download Burp Suite

You can download the Burp Suite JAR file from two places. Both options give you the same JAR format, so pick whichever is easier for you. The goal is to get a `.jar` file, not a Windows `.exe` installer.

<details>
<summary><strong>Quick download using the command line</strong></summary>

My terminal is already open in the same folder. If you prefer using the terminal, you can download the JAR file with `curl`. Open PowerShell or Command Prompt inside your `burpsuite` folder and run:

```powershell
curl "https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar" -o burpsuite_desktop_v2026.10.1.jar
```

This command saves the JAR file to your current folder. You can change the output name after `-o` if you want a different filename.

Be patient, the file is approximately `750 MB` in size.

### Verify the download from the terminal

You can match the checksum to make sure the file downloaded correctly:

```powershell
Get-FileHash .\burpsuite_desktop_v2026.10.1.jar -Algorithm SHA256
```

If the hash matches the value below, you are good to go:

```
sha256:e8ab086537b1643b91ca09d2fc2a6c3e08a8bae0c85280797c5c9ec76506c3c5
```

</details>

**Option 1: Official Download from PortSwigger**

[Download Burp Suite from PortSwigger](https://portswigger.net/burp/releases)

1. Open the download page.
2. Select the latest Professional or Community release.
3. Choose the standalone **JAR** format.
4. Save the `.jar` file to your Downloads folder.

**Option 2: Direct Download from Project Releases**

If you want to skip the format selection and avoid any confusion, use the ready-made JAR files hosted on this project:

[Download Burp Suite JAR from Project Releases](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/Professional_and_Community)

Direct download link for the latest JAR:

[burpsuite_desktop_v2026.10.1.jar](https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar)

1. Open the release page or the direct link.
2. Download the `.jar` file.
3. Save it to your Downloads folder or any folder you prefer.

**Important:** Choose the JAR format, not the Windows `.exe` installer, for this Java-based setup. The project release already provides the correct JAR format, so beginners can download it without worrying about picking the right file type.

## 3. Download BurpLoader

BurpLoader is the small launcher that starts Burp Suite. Download it the same way you downloaded the JAR file, from either the release page or the direct link. Both options give you the same file.

<details>
<summary><strong>Quick download using the command line</strong></summary>

If your terminal is still open inside the `burpsuite` folder, run:

```powershell
curl "https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar" -o burp-loader.jar
```

This command saves `burp-loader.jar` to your current folder. Be patient, it is a small file but the download depends on your connection.

### Verify the download from the terminal

You can match the checksum to make sure the file downloaded correctly:

```powershell
Get-FileHash .\burp-loader.jar -Algorithm SHA256
```

If the hash matches the value below, you are good to go:

```
sha256:1fa388f0c102c7c11ed8bf239f10ae2cefd05dcf6c855820b475d2fb297e767e
```

</details>

**Option 1: Download from the release page**

[Download BurpLoader from the v1.0 Release](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0)

1. Open the release page.
2. Find `burp-loader.jar` in the assets list.
3. Download it and save it to your `burpsuite` folder.

**Option 2: Direct download**

[burp-loader.jar](https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar)

1. Open the direct link.
2. Download the `.jar` file.
3. Save it to your `burpsuite` folder.

## 4. Confirm Your Files Are in Place

Before we start setting things up, check that both files are in the same folder. Inside your `burpsuite` folder, run:

```powershell
ls
```

You should see both files listed:

```powershell
    Directory: C:\Users\octob\<USERNAME>\burpsuite

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        15-11-2026  07:07 PM        1238721 burp-loader.jar
-a----        15-11-2026  06:52 PM      751385742 burpsuite_desktop_v2026.10.1.jar

PS C:\Users\octob\<USERNAME>\burpsuite>
```

If both files are downloaded, you are all set. Now we can start setting it up.

## 4. Launch BurpLoader

Now let's start BurpLoader and launch Burp Suite.

<details>
<summary><strong>If BurpLoader finds Burp Suite automatically</strong></summary>

Run BurpLoader and wait a moment. If both Burp Suite and BurpLoader are in the same folder, BurpLoader will locate Burp Suite on its own and show a `ready to start` message. You can then hit **Run** directly.

<img width="1287" height="583" alt="ready to start" src="https://github.com/user-attachments/assets/e0d611cf-fa0f-44b2-b216-82cb224858be" />

</details>

<details>
<summary><strong>If BurpLoader does not find Burp Suite automatically</strong></summary>

In this case, if you installed BurpLoader and Burp Suite in different folders, or BurpLoader was not able to detect it even in the same location, use the **Browse** button to locate the Burp Suite JAR file manually.

<img width="1283" height="582" alt="browse for burpsuite jar" src="https://github.com/user-attachments/assets/2be23875-c670-4188-96bf-2297320f99df" />

Once you select the Burp Suite JAR with Browse, BurpLoader will show that Burp Suite was selected successfully. Hit **Run** and let's go.

<img width="1287" height="584" alt="burpsuite selected successfully" src="https://github.com/user-attachments/assets/5b00a8d6-7ba0-4d23-9d38-4152815950f7" />

</details>

When you press **Run**, be patient. The first launch of Burp Suite can take about 30 seconds to open, so do not spam the Run button.

<details>
<summary><strong>Choosing Professional or Community on launch</strong></summary>

When Burp Suite launches, it will ask you to continue with Professional or Community. The latest version of Burp Suite from PortSwigger ships both Community and Professional in one package. On older versions, both were shipped separately. So no matter whether you run an old version or a new one, it works the same way. Right now, continue with Professional.

<img width="626" height="860" alt="choose professional or community" src="https://github.com/user-attachments/assets/862ad6ac-616f-41de-bf27-8322964a887e" />

</details>

Once all the preparation is done and Burp Suite launches, you are ready to go.

## 5. Setting Up the License

Now we need to activate Burp Suite. BurpLoader will generate the license for you.

### Step 1: Copy the generated license

Copy the generated license from BurpLoader and paste it into the Burp Suite license window, then hit **Next**.

<img width="1708" height="680" alt="no license pasted" src="https://github.com/user-attachments/assets/ddbe7fb5-9397-4486-9bab-c4ce0bd1a110" />

### Step 2: Choose manual activation

After hitting **Next**, Burp Suite opens a new window. Click on **Manual activation** and hit **Next**.

<img width="610" height="632" alt="manual activation" src="https://github.com/user-attachments/assets/50d7efa1-3dde-4370-973e-a73ee9bef9f1" />

### Step 3: Copy the request into BurpLoader

Burp Suite will show an activation request. Copy that request from Burp Suite and paste it into the **Activation Request** tab in BurpLoader.

<img width="1669" height="629" alt="activation request tab" src="https://github.com/user-attachments/assets/b0d10364-8b71-479b-87bd-fafe7d5f78d8" />

### Step 4: Paste the response back into Burp Suite

BurpLoader will generate an activation response. Copy the activation response from BurpLoader, paste it into Burp Suite in the **Paste response** field, and hit **Next**.

<img width="1677" height="644" alt="activation response" src="https://github.com/user-attachments/assets/bbae035f-affe-4756-9c31-3ff3c37a3910" />

Your license will now be activated.

<img width="602" height="618" alt="license activated" src="https://github.com/user-attachments/assets/e84844c3-0e5f-4234-a321-bc00b0ca4e49" />

## 6. Reopening Burp Suite

If you want to open Burp Suite again later, repeat the launch step. You have two easy options:

**Option 1:** Double click on `burp-loader.jar` to open BurpLoader, then press **Run**.

**Option 2:** Use the terminal and run:

```powershell
java -jar burp-loader.jar
```

When the prompt appears, hit **Run** to reopen Burp Suite. After Burp Suite starts, you can close BurpLoader.

<img width="952" height="690" alt="reopen burpsuite" src="https://github.com/user-attachments/assets/145f59b7-f125-4c5d-81ce-55ce3969231c" />

And that is it. Burp Suite is installed, activated, and ready for your authorized security testing and educational labs.



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

