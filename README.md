# BurpSuite Pro 2026 Loader (Windows, Linux, Mac)

**The ultimate Burp Suite Professional Loader and Activator. Cross-platform support for Windows, Linux, and macOS with Java 21-25 compatibility.**

This project provides a lightweight, high-performance GUI loader for Burp Suite Professional. It is designed for security researchers, penetration testing learners, and controlled lab environments. The loader automatically bypasses the license check, allowing you to run Burp Suite Pro on modern Java environments seamlessly.

The tool is built with a focus on reliability, ease of setup, and cross-platform compatibility. It includes built-in tools to generate the license key, handle manual activation, and even create a 1-click desktop shortcut for future use.

![Burp Suite Pro Loader UI](https://github.com/user-attachments/assets/e21759d4-6b20-471c-bfa0-5c5d1559f91a)

## Features

- **Latest 2026 Build:** Fully compatible with modern Burp Suite versions.
- **Cross-Platform:** Works natively on Windows, Linux (Ubuntu, KDE, XFCE), and macOS.
- **Modern Java Support:** Tested and working on Java 21, 22, 23, 24, and 25.
- **1-Click Desktop Shortcut:** Automatically generates a shortcut with the custom logo so you don't have to open the loader every time.
- **Built-in Activation UI:** Paste the Burp activation request directly into the loader to instantly generate the response and license key.
- **Clear License Feature:** A built-in button to completely wipe the Burp license from the system (Registry/AppData) if you need to re-activate.
- **Auto-Detect:** Automatically finds the Burp Suite JAR in the same folder.

## Tested Environments

- Windows 10 / 11 (64-bit)
- Linux (Ubuntu, Kali, KDE, XFCE)
- macOS (Intel and Apple Silicon)

## Windows Setup

### Requirements
- Windows 64-bit
- Java 21 or newer
- Official Burp Suite JAR file

**Install Java**
Download and install Java 21 for Windows:
[Java 21 Download](https://download.oracle.com/java/21/archive/jdk-21.0.9_windows-x64_bin.msi)

### Download Burp Suite
Download the latest Burp Suite release from the official source:
[https://portswigger.net/burp/releases](https://portswigger.net/burp/releases)

Select:
- Burp Suite Professional
- JAR format

### Download BurpLoader
[Click here to download burp-loader.jar](https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar)

### Workspace Preparation
Create a dedicated folder to store Burp Suite files. For example:
`C:\Users\<USERNAME>\Documents\Burp`

Move both the `burp-loader.jar` and the `burpsuite_pro.jar` into this directory.

### Launch Burp Suite
Open PowerShell or Command Prompt in the directory where the JAR files are stored.

Run the loader using Java:
```powershell
java -jar .\burp-loader.jar
```

The Loader GUI will open.
1. Click **Browse...** and select your Burp Suite JAR file.
2. Click **Run**.

## Activation Process

When prompted by Burp Suite for a license, follow these steps to activate it using the loader.

### 1. Accept License Agreement
On the first launch, review and accept the Burp Suite license Agreement to proceed.

### 2. Paste License Key
When prompted for a license, click the **Copy License** button in the Loader GUI. Paste it into Burp Suite and click Next.

### 3. Manual Activation
On the License Activation page, click **Manual Activation** at the bottom.

### 4. Paste Request
Copy the request from Burp Suite and paste it into the **Activation Request** box in the Loader GUI.

### 5. Copy Response
Copy the generated response from the Loader GUI and paste it into Burp Suite.

### 6. Finish
Click Finish and enjoy Burp Suite Pro.

### 7. Create Shortcut (Optional)
To avoid opening the loader every time, click the **Create Shortcut** button in the Loader GUI. This will place a custom Burp Suite Pro icon on your Desktop. You can use this shortcut to launch Burp directly.

## Linux Setup

### Requirements
- Linux 64-bit (Ubuntu, Kali, KDE, XFCE)
- Java 21 or newer
- Official Burp Suite JAR file

**Install Java**
```bash
sudo apt update
sudo apt install openjdk-21-jdk -y
```

Verify Java is installed:
```bash
java -version
```

### Download Burp Suite
Download the latest Burp Suite JAR from the official source:
[https://portswigger.net/burp/releases](https://portswigger.net/burp/releases)

### Download BurpLoader
Download the loader via terminal:
```bash
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
```

### Workspace Setup
Create a workspace folder:
```bash
mkdir -p /home/$USER/Documents/burp
```

Move the JAR files:
```bash
mv /home/$USER/Downloads/burpsuite_*.jar /home/$USER/Documents/burp/
mv /home/$USER/Downloads/burp-loader.jar /home/$USER/Documents/burp/
cd /home/$USER/Documents/burp
```

### Run Burp Suite
```bash
java -jar burp-loader.jar
```

The rest of the activation process is identical to the Windows steps above.

**Note on Linux Shortcuts:** When you click "Create Shortcut", the launcher is added to your **Application Menu** (Show Applications). You can drag it to your taskbar or desktop from there.

## macOS Setup

### Requirements
- macOS (Intel or Apple Silicon)
- Java 21 or newer
- Official Burp Suite JAR file

**Install Java**
You can install Java 21 using Homebrew:
```bash
brew install openjdk@21
```

### Download Burp Suite
Download the latest Burp Suite JAR from the official source:
[https://portswigger.net/burp/releases](https://portswigger.net/burp/releases)

### Download BurpLoader
Download the loader via terminal:
```bash
curl -L -O https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
```

### Run Burp Suite
Open Terminal and run:
```bash
java -jar burp-loader.jar
```

**Note on Mac Shortcuts:** When you click "Create Shortcut", a `.command` file is created on your Desktop. If macOS blocks it the first time, simply right-click the file and select **Open** to trust it.

## Legal Disclaimer

This tool is for educational and authorized security testing purposes only. The author is not responsible for any misuse or damage caused by this software.

## Thank You for the Support

Big thanks to everyone who has starred this repo and is using this project. Seeing your support, feedback, and interest is what keeps this going. Appreciate every single one of you.
```
