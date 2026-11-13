#### Ubuntu Setup

A step-by-step guide to setting up Burp Suite Professional on Ubuntu.

**Tested Environment:** Ubuntu 26.04.1 LTS

##### Step 1: Install Java

Before getting started, let's install Java.

For this demo, we're using **OpenJDK 21**. BurpLoader supports Java 11–26, but we recommend **Java 21 or 25** for Burp Suite compatibility.

Open your terminal and run:

```bash
sudo apt update
sudo apt install openjdk-21-jdk -y
```

##### Step 2: Verify Java Installation

Once the installation is complete, verify that Java and the Java compiler are installed correctly.

```bash
java -version
javac -version
```

If everything is installed correctly, both commands should display their respective version information.

**Expected Output:**

<div align="center">
 <img alt="java install" src="https://github.com/user-attachments/assets/87d2143f-0716-4d8c-9d21-11966cd19cda">
</div>

<div align="center">
 <sub>Figure 1: Verifying Java and Java Compiler installation on Ubuntu.</sub>
</div>

##### Step 3: Download BurpLoader

Now it's time to download BurpLoader!

You can download it directly from the GitHub release: [**Download burp-loader.jar**](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0)

Or, if you're lazy like me and prefer the terminal, use `wget` to download it directly.
```bash
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
```

For this demonstration, I'm using the **Desktop** directory to keep everything organized and easy to access. Feel free to save BurpLoader and your Burp Suite installer anywhere you prefer.

##### Step 4: Get Burp Suite Ready

Now for the main ingredient: **Burp Suite!** 🍔

You can download Burp Suite directly from the official PortSwigger website. I've also added the latest stable release to this repository's GitHub Releases, so if you're lazy like me and don't want to hunt for download links, I've got you covered!

**Option 1: Download from GitHub Releases**

You can download the version included in this repository directly using `wget`:

```bash
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar
```

I'll try to keep the repository updated with stable releases whenever possible, so you don't have to search for them manually.

**Option 2: Download from the Official Website**

Prefer downloading directly from the source? No problem!

Visit the official [PortSwigger Burp Suite Releases](https://portswigger.net/burp/releases) page to find the latest available version.

**Important: Select the JAR format**

When downloading Burp Suite, make sure to select `JAR` from the platform dropdown before clicking the Download button.

<div align="center">
  <img alt="Select JAR format from PortSwigger download options" src="https://github.com/user-attachments/assets/93c5e8d0-87e8-4a50-9aa7-b5e4b1738e84">
</div>

<div align="center">
  <sub>Figure 2: Select the JAR package before downloading Burp Suite.</sub>
</div>

The JAR package runs across supported operating systems using a compatible Java runtime. We'll use the same download format for `Windows`, `Ubuntu`, `Kali Linux` and `macOS`.

##### Step 5: Configure Burp Suite

Now that everything is downloaded, let's get Burp Suite up and running!

**1. Locate Burp Suite**

If both BurpLoader and Burp Suite are saved in the same folder, BurpLoader should automatically detect Burp Suite and display the **Ready to Start** status.

<div align="center">
  <img alt="BurpLoader ready to start interface" src="https://github.com/user-attachments/assets/c387240d-8a69-41a4-b880-5ea544b4c8f2">
</div>

<div align="center">
  <sub>Figure 3: BurpLoader detecting the downloaded Burp Suite JAR file.</sub>
</div>

If BurpLoader cannot find Burp Suite, simply click the **Browse** button and manually locate your downloaded Burp Suite JAR file.

**Tip:** If you opened BurpLoader before downloading Burp Suite, simply restart BurpLoader after downloading it.

**2. Launch Burp Suite**

Once Burp Suite is detected, click the **Run** button to launch the application.

Be patient! The first startup may take a little longer than usual. Give it a moment to initialize.

If a JRE warning appears, simply ignore it and continue with the setup.

<div align="center">
  <img alt="BurpLoader application launch" src="https://github.com/user-attachments/assets/a3ab4cfa-c617-4fa5-a8c6-2cb8f7a7532a">
</div>

<div align="center">
  <sub>Figure 4: Starting Burp Suite from the application interface.</sub>
</div>

**3. Accept the Terms and Conditions**

When Burp Suite starts for the first time, you'll be presented with the Terms and Conditions.

Read through them and accept the terms to continue.

<div align="center">
  <img alt="Burp Suite terms and conditions" src="https://github.com/user-attachments/assets/fb2e97f8-bb74-421f-8112-ae3e62eb76c9">
</div>

<div align="center">
  <sub>Figure 5: Accepting the Burp Suite Terms and Conditions.</sub>
</div>

**4. Select Burp Suite Professional**

On the next screen, select **Continue with Professional**.

<div align="center">
  <img alt="Continue with Burp Suite Professional" src="https://github.com/user-attachments/assets/5ae8923f-19b2-45a8-be33-58293224edb3">
</div>

**5. Copy The License From Loader Past in Burpsuite like this and click on next**

<div align="center">
  <img width="1775" height="912" alt="image" src="https://github.com/user-attachments/assets/e44a9923-8921-4e92-a85b-1389e7f3b0ad" />
</div>

<div align="center">
  <sub>Figure 7: Pasting the copied license key into Burp Suite.</sub>
</div>

**6. Select Manual Activation**

Click on **Manual activation** to proceed with the manual activation process.

<div align="center">
  <img alt="Burp Suite manual activation" src="https://github.com/user-attachments/assets/d88aee9f-9ccc-4b45-898e-882e7958af82">
</div>

**7. Copy The Request from Burpsuite paste In bruploader:**

<div align="center">
  <img width="1790" height="906" alt="image" src="https://github.com/user-attachments/assets/8a905018-8ec2-415a-bddd-dfd1c00ecad9" />
</div>

**8. Copy The Copy Response from burploader Paste in Burpsuite and click Next:**

<div align="center">
  <img width="1746" height="929" alt="image" src="https://github.com/user-attachments/assets/bfa7c13c-221f-4046-ada7-c5899cf59660" />
</div>


**That it ur License is activated enojy ur burpsuit:**

<div align="center">
  <img width="1774" height="933" alt="image" src="https://github.com/user-attachments/assets/76b9d431-f143-4f00-8c78-de27085edae8" />
</div>

<div align="center">
  <sub>Figure 11: License successfully activated and Burp Suite ready to use.</sub>
</div>

**9. To create a shortcut, click on Create Shortcut button:**

<div align="center">
  <img width="1075" height="769" alt="image" src="https://github.com/user-attachments/assets/88c1ad4c-8749-4e65-8583-ecf327c233ef" />
</div>

> If u create shortcut without activating burpsuit it will open unconfig burp, if u configed it click yes

<div align="center">
  <img width="580" height="184" alt="image" src="https://github.com/user-attachments/assets/a160b5b4-7db3-4ddc-9123-dc55bcacd73a" />
</div>

Your burpsuite pro will be added to ur application launcher

<div align="center">
  <img width="1608" height="592" alt="image" src="https://github.com/user-attachments/assets/788a84ba-d5c1-45a0-8dc8-ef5584545ae4" />
</div>

by right clicking it u can pin it to dock and close rest of ur burploader and terminal with single click ur burpsuit pro will be ready

<div align="center">
  <img width="1918" height="1049" alt="image" src="https://github.com/user-attachments/assets/01ef18c2-509b-44e0-93ca-e12af2a6ee08" />
</div>



 # BurpSuite-Toolkit

## About the Project

## Features

## Supported Platforms

## Tested Environments

## Installation Guide

### 1. Windows Installation
[Coming Soon]

### 2. Linux Installation
 










#### Kali Linux Setup
[Coming Soon]

### 3. macOS Installation
[Coming Soon]

## Usage Guide

## Screenshots

## Troubleshooting

## Disclaimer

## License


## Faq

Burploader support java11-java 25 run and tested 
but current burpsuit support and run most stable on java 21 and java 17 , in future if burpsuit make say there burpsuit support and fulltest on java 25 still the burploader will be able to work im not sure about java 27 as they change maybe it will work or if it not work ill reopen the project and maintian it 


Most people downloading the wrong version of burpsuit in there system for all os .Jar version will sipport if u download burpsuit setup accoidng to ur system like .exe , .deb or x64 , arm the burploader will not be able to work for all os burpsuit.jar formate is applicate and this single burploader.jar will work on all os as so far i have tested.

I saw many people dm me on linked and created issue in github , so i add button in loder which u can use to dowload burploader form my releas or offical release till last year Portwigger launch 
communtiy and professional version diffectly but right now they launch single version which contian both community and professional , i guess they gonna release pro and comminute version together from now onward , anyway both version work exactly same and u cant use burp ai bez u have to login into web portal of portwsigger to use that so im not skill full enoght to do that right now, if u guys able to do it please dont forget to teach me 
