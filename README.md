
# BurpSuite Pro 2026 Loader (Windows, Linux, Mac)

**The ultimate Burp Suite Professional Loader and Activator. Cross-platform support for Windows, Linux, and macOS with Java 21-25 compatibility.**

## ⬇️ Download
**[Click here to download the latest BurpLoader (v1.0)](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0)**

---

## What This Tool Does
This project provides a lightweight, high-performance GUI loader for Burp Suite Professional. It is designed for security researchers, penetration testing learners, and controlled lab environments. The loader automatically bypasses the license check, allowing you to run Burp Suite Pro on modern Java environments seamlessly.

The tool is built with a focus on reliability, ease of setup, and cross-platform compatibility. It includes built-in tools to generate the license key, handle manual activation, and even create a 1-click desktop shortcut for future use.

![Burp Suite Pro Loader UI](https://github.com/user-attachments/assets/e21759d4-6b20-471c-bfa0-5c5d1559f91a)

## Tested Platforms
- **Windows:** 10 / 11 (64-bit)
- **Linux:** Ubuntu, Kali, KDE, XFCE (64-bit)
- **macOS:** Intel and Apple Silicon (M1/M2/M3)

---

## Installation & Setup

### Windows Setup
**Requirements:** Windows 64-bit, Java 21 or newer, Official Burp Suite JAR file.

1. **Install Java:** Download and install [Java 21 for Windows](https://download.oracle.com/java/21/archive/jdk-21.0.9_windows-x64_bin.msi).
2. **Download Burp Suite:** Go to the official [PortSwigger Releases](https://portswigger.net/burp/releases) page. Select **Burp Suite Professional** and choose the **JAR** format.
3. **Download BurpLoader:** Download `burp-loader.jar` from the [Releases page](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0).
4. **Workspace Preparation:** Create a folder (e.g., `C:\Users\<USERNAME>\Documents\Burp`) and move both the `burp-loader.jar` and `burpsuite_pro.jar` into it.
5. **Launch:** Open PowerShell in that folder and run:
   ```powershell
   java -jar .\burp-loader.jar
   ```
6. **Run Burp:** In the Loader GUI, click **Browse...** to select the Burp Suite JAR, then click **Run**.

### Linux Setup
**Requirements:** Linux 64-bit, Java 21 or newer, Official Burp Suite JAR file.

1. **Install Java:**
   ```bash
   sudo apt update
   sudo apt install openjdk-21-jdk -y
   ```
2. **Download Burp Suite:** Get the JAR from the official [PortSwigger Releases](https://portswigger.net/burp/releases).
3. **Download BurpLoader:**
   ```bash
   wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
   ```
4. **Workspace Preparation:**
   ```bash
   mkdir -p /home/$USER/Documents/burp
   mv /home/$USER/Downloads/burpsuite_*.jar /home/$USER/Documents/burp/
   mv /home/$USER/Downloads/burp-loader.jar /home/$USER/Documents/burp/
   cd /home/$USER/Documents/burp
   ```
5. **Launch:**
   ```bash
   java -jar burp-loader.jar
   ```

### macOS Setup
**Requirements:** macOS, Java 21 or newer, Official Burp Suite JAR file.

1. **Install Java:**
   ```bash
   brew install openjdk@21
   ```
2. **Download Burp Suite:** Get the JAR from the official [PortSwigger Releases](https://portswigger.net/burp/releases).
3. **Download BurpLoader:**
   ```bash
   curl -L -O https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
   ```
4. **Launch:** Open Terminal and run:
   ```bash
   java -jar burp-loader.jar
   ```

---

## Activation Process

Once Burp Suite opens via the loader, follow these steps to activate it:

1. **Accept License:** Review and accept the Burp Suite license Agreement.
2. **Paste License Key:** In the Loader GUI, click **Copy License**. Paste it into Burp Suite and click Next.
3. **Manual Activation:** On the License Activation page in Burp, click **Manual Activation** at the bottom.
4. **Paste Request:** Copy the request from Burp and paste it into the **Activation Request** box in the Loader GUI.
5. **Copy Response:** Copy the generated response from the Loader and paste it into Burp Suite.
6. **Finish:** Click Finish and enjoy Burp Suite Pro.

**Optional:** Click **Create Shortcut** in the Loader GUI to place a custom icon on your Desktop. You can use this shortcut to launch Burp directly next time without opening the loader.

---

## Features & Updates

- **Latest 2026 Build:** Fully compatible with modern Burp Suite versions.
- **Modern Java Support:** Tested and working on Java 21, 22, 23, 24, and 25.
- **Cross-Platform:** Works natively on Windows, Linux (Ubuntu, KDE, XFCE), and macOS.
- **1-Click Desktop Shortcut:** Automatically generates a shortcut with the custom logo.
- **Built-in Activation UI:** Paste the Burp activation request directly into the loader to instantly generate the response.
- **Clear License Feature:** A built-in button to completely wipe the Burp license from the system if you need to re-activate.
- **Auto-Detect:** Automatically finds the Burp Suite JAR in the same folder.

---

## Legal Disclaimer
This tool is for educational and authorized security testing purposes only. The author is not responsible for any misuse or damage caused by this software.

## Thank You for the Support
Big thanks to everyone who has starred this repo and is using this project. Seeing your support, feedback, and interest is what keeps this going. Appreciate every single one of you.
```
