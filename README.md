<div align="center">

# BurpSuite 2026 Loader

<img
  width="180"
  alt="BurpSuite Toolkit Logo"
  src="https://github.com/user-attachments/assets/5f1e1607-96f1-4703-9589-21d07c4fecf1"
/>

**A lightweight, cross-platform Java utility for simplifying Burp Suite setup in educational labs and authorized security testing.**

![Latest](https://img.shields.io/badge/LATEST-v1.0.0-16a34a?style=plastic)
![Legacy](https://img.shields.io/badge/LEGACY-v0.9-ea580c?style=plastic)
![Platforms](https://img.shields.io/badge/PLATFORMS-Windows%20%7C%20Linux%20%7C%20macOS-2563eb?style=plastic)
![Documentation](https://img.shields.io/badge/DOCUMENTATION-Available-9333ea?style=plastic)

</div>

## Available Versions

Choose the release that best suits your needs.

| Version | Status | Description | Release |
|---|---|---|---|
| **v1.0.0** | 🟢 Latest | Updated interface, improved JAR detection and desktop shortcut management. | [View Release](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0) |
| **v0.9** | 🟠 Legacy | Original edition featuring the earlier interface and manual workflow. | [View Release](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v0.9) |

> **New here?** Start with the latest release for the most recent improvements.

## About the Project

BurpSuite 2026 Loader is a lightweight, cross-platform Java utility designed to simplify Burp Suite setup and launching.

This repository includes installation guides, compatibility details, and practical resources for beginners and security enthusiasts interested in web application security testing.

## Features

- **Burp Suite Compatibility:** Supports modern and legacy versions.
- **Lightweight:** Under 2 MB. No bulky installer.
- **Pure Java:** Runs as a single JAR application.
- **Cross-Platform:** Supports Windows, Linux and macOS.
- **GUI-First:** Simple point-and-click interface.
- **Automatic JAR Detection:** Finds Burp Suite JAR files automatically.
- **Manual JAR Selection:** Browse and select JAR files from any directory.
- **Application Launchers:** Create desktop shortcuts on Windows and application launchers on Linux and macOS.
- **Built for Research:** Designed for educational labs and authorized security testing.

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

**Reported compatibility range:** Java 11–26 (not every version individually tested).

macOS testing is still pending. Unfortunately, the Mac left this world before testing could begin. 💀

## What's New in v1.0.0

### New Features

- **Java Compatibility:** Expanded runtime compatibility.
- **JAR Detection & Browse:** Automatically detects Burp Suite JAR files or lets you select one manually.
- **Official Download Links:** Quick access to PortSwigger's official Community and Professional downloads.
- **Application Launchers:** Create desktop shortcuts on Windows and application launchers on Linux and macOS.

### UI & Experience

- Refreshed interface with a cleaner, responsive layout.
- Embedded application icons.
- **Copy & Paste Buttons:** Less manual work, more laziness. 💀

## Installation Guides

| Operating System | Installation Guide |
|---|---|
| **Windows 10 / 11** | [View Guide](#windows-installation) |
| **Ubuntu / Kali Linux** | [View Linux Guide](doc/Setup-guide/Linux) |

---

### Windows

Follow this step-by-step guide to set up Burp Suite on Windows 10 or 11.

#### Requirements

- Windows 10 or Windows 11 (64-bit)
- Java 21 or Java 25 (recommended)
- Internet connection

#### 1. Install Java

Download Java 21 or Java 25 for Windows:

- [Download Java 21 (Windows x64)](https://download.oracle.com/java/21/archive/jdk-21.0.9_windows-x64_bin.msi)
- [Download Java 25 (Windows x64)](https://www.oracle.com/java/technologies/javase/jdk25-archive-downloads.html)

Open the downloaded `.msi` installer, follow the setup wizard, and complete the installation.

#### Verify Java Installation

Open PowerShell or Command Prompt and run:

```powershell
java -version
```

If Java is installed correctly, you'll see the installed version displayed in the terminal.

<details>
<summary><strong>1.1 Organize Your Files (For Beginners)</strong></summary>

Let's keep everything in one place before downloading anything. I'm using the Documents folder because I don't like a messy Desktop. You can choose any folder you prefer.

Create a folder named `burpsuite` inside Documents:

```powershell
cd "$HOME\Documents"
mkdir burpsuite
cd burpsuite
```

Your terminal is now inside the folder where you can keep your Burp Suite files.

</details>

---
#### 2. Download Burp Suite

Download Burp Suite from the official PortSwigger website. This launcher requires the **standalone JAR format**.

<details>
<summary><strong>Option 1: Download the recommended version (Recommended)</strong></summary>

[Download Burp Suite 2026.10.1](https://portswigger.net/burp/releases/professional-community-2026-10-1)

1. Open the download page.
2. Select Community or Professional Edition.
3. Find the available download formats.
4. **Choose the standalone JAR file only.**
5. Save the downloaded `.jar` file in your `burpsuite` folder.

</details>

<div align="center">
  <img
    width="100%"
    alt="PortSwigger Burp Suite download page showing the JAR format selected"
    src="https://github.com/user-attachments/assets/0c068f6a-9818-43b4-b283-82205ad2279d"
  />
</div>

> **Important:** This launcher supports `.jar` files only. Windows `.exe`, `.msi`, and other platform-specific installers are not supported. Make sure you select the JAR format before downloading.

---

#### 3. Download BurpLoader

BurpLoader is the Java-based launcher included in this project.

[View BurpLoader v1.0 Release](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0)

Check the release assets for the application JAR file.

---

<details>
<summary><strong>3.1 Organize Your Files (For Beginners)</strong></summary>

Before continuing, make sure both downloaded files are inside the `burpsuite` folder you created earlier in your Documents directory.

If they are in your Downloads folder, move them into:

`Documents\burpsuite`

Your folder should contain the required application files before proceeding.

</details>

#### 4. Launch BurpLoader

Navigate to your `burpsuite` folder and double-click `burp-loader.jar` to launch it.

**Alternatively,** open PowerShell or Command Prompt inside the folder and run:

```powershell
java -jar burp-loader.jar
```

If Burp Suite and BurpLoader are in the same folder, BurpLoader should detect the JAR automatically and display a **Ready to Start** message.

<div align="center">
  <img width="100%" alt="BurpLoader showing the Ready to Start status" src="https://github.com/user-attachments/assets/e0d611cf-fa0f-44b2-b216-82cb224858be" />
</div>

> **Note:** After clicking **Run**, Burp Suite may take around **10–30 seconds** to launch, depending on your system configuration. Please wait and avoid clicking **Run** repeatedly, as this may open multiple Burp Suite windows.

Once Burp Suite launches, you'll be prompted to choose between **Professional** and **Community** editions. Select **Professional** to continue.

---

<div align="center">
  <img width="626" alt="Burp Suite Professional or Community edition selection screen" src="https://github.com/user-attachments/assets/862ad6ac-616f-41de-bf27-8322964a887e" />
</div>

---

<details>
<summary><strong>Having trouble with automatic detection? Use Browse.</strong></summary>

If Burp Suite is stored in a different folder or automatic detection fails, use the **Browse** button to locate its JAR file manually.

<div align="center">
  <img width="100%" alt="BurpLoader Browse button for selecting a Burp Suite JAR" src="https://github.com/user-attachments/assets/2be23875-c670-4188-96bf-2297320f99df" />
</div>

After selecting the JAR file, confirm that it is detected successfully.

<div align="center">
  <img width="100%" alt="BurpLoader showing the selected Burp Suite JAR" src="https://github.com/user-attachments/assets/5b00a8d6-7ba0-4d23-9d38-4152815950f7" />
</div>

</details>

---

### 5. Setting Up the License

#### Step 1: License Entry

Paste the key generated by BurpLoader into the **Burp Suite Activation** window and click **Next**.

<div align="center">
  <img width="100%" alt="Burp Suite license entry window" src="https://github.com/user-attachments/assets/ddbe7fb5-9397-4486-9bab-c4ce0bd1a110"/>
</div>

---

#### Step 2: Choose Manual Activation

After clicking **Next**, Burp Suite opens a new window. Select **Manual activation** and click **Next**.

<div align="center">
  <img width="610" alt="Burp Suite manual activation option" src="https://github.com/user-attachments/assets/50d7efa1-3dde-4370-973e-a73ee9bef9f1" />
</div>

---
#### Step 3: Activation Request

Burp Suite will display an activation request. Copy the request and paste it into the **Activation Request** tab in BurpLoader.

<div align="center">
  <img width="100%" alt="Burp Suite activation request interface" src="https://github.com/user-attachments/assets/b0d10364-8b71-479b-87bd-fafe7d5f78d8" />
</div>

---
#### Step 4: Activation Response

BurpLoader will generate an activation response. Copy the response, paste it into the **Paste Response** field in Burp Suite, and click **Next**.

<div align="center">
  <img width="100%" alt="Burp Suite activation response window" src="https://github.com/user-attachments/assets/bbae035f-affe-4756-9c31-3ff3c37a3910" />
</div>

---

Your Burp Suite activation is complete.

<div align="center">
  <img width="602" alt="Burp Suite activation completed successfully" src="https://github.com/user-attachments/assets/e84844c3-0e5f-4234-a321-bc00b0ca4e49" />
</div>

---

### 6. Reopening Burp Suite

Want to use Burp Suite again later? You can reopen it using either of these methods.

**Option 1: Double-click**

1. Open your `burpsuite` folder.
2. Double-click `burp-loader.jar` to launch BurpLoader.
3. Click **Run** to start Burp Suite.

**Option 2: Use the terminal**

Open PowerShell or Command Prompt in the `burpsuite` folder and run:

```powershell
java -jar burp-loader.jar
```

When BurpLoader opens, click **Run** to start Burp Suite.

<div align="center">
  <img width="100%" alt="BurpLoader interface showing the Run option" src="https://github.com/user-attachments/assets/d73b5a49-7a72-4486-a6f3-168950dbd846" />
</div>

That's it! Burp Suite is ready for your authorized security testing and educational labs.

### 7. Create a Shortcut (Windows)

Opening BurpLoader every time can be inconvenient. You can simplify this by creating a desktop shortcut directly from BurpLoader.

1. Open BurpLoader.
2. Click **Create Shortcut**.
3. When the confirmation prompt appears, click **Yes**.

<div align="center">
  <img width="100%" alt="BurpLoader Create Shortcut button" src="https://github.com/user-attachments/assets/c8435eae-a681-46a7-80e1-7e4a70803246" />
</div>

The shortcut will appear on your Windows desktop. Double-click it whenever you want to launch Burp Suite.

<div align="center">
  <img width="233" alt="Burp Suite desktop shortcut" src="https://github.com/user-attachments/assets/eeadee22-6657-405c-b887-ae5368f4645c" />
</div>

> **Note:** Configure Burp Suite before creating the shortcut. Otherwise, the shortcut may launch an unconfigured instance. Clearing the licence may also remove the desktop shortcut.

Enjoy, and happy testing!

## FAQ

### 1. Which Java versions does BurpLoader support?

BurpLoader supports Java 17–26. Burp Suite has been tested with Java 17, Java 21, and Java 25.

For the best experience, use one of the tested Java versions.

### 2. Which operating systems and Burp Suite formats are supported?

BurpLoader supports Windows, Linux, and macOS, but works only with Burp Suite's standalone `.jar` file.

Other installation formats, such as `.exe`, `.msi`, and `.deb`, are not supported.

### 3. Can the legacy v0.9 run newer Burp Suite versions?

Yes. Both older and latest Burp Suite versions run perfectly with Java 21.

**Important:** Legacy BurpLoader v0.9 does not properly support Java versions newer than 21. If you download Java 25 or another newer version, you may experience compatibility issues.

**For v0.9, download Java 21 only. Do not download Java 25 or newer.**

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
