# Burp Suite Professional Setup on Ubuntu

![Tested](https://img.shields.io/badge/Tested-Ubuntu%2026.04.1%20LTS-2D2D2D?style=flat&logo=ubuntu&logoColor=E95420)
![Java](https://img.shields.io/badge/Java-21-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Package](https://img.shields.io/badge/Package-JAR-2D2D2D?style=flat&logo=java&logoColor=white)

A beginner-friendly, step-by-step guide to installing and configuring Burp Suite on Ubuntu.

## Table of Contents

- [Step 1: Install Java](#step-1-install-java)
- [Step 2: Verify Java Installation](#step-2-verify-java-installation)
- [Step 3: Download BurpLoader](#step-3-download-burploader)
- [Step 4: Get Burp Suite Ready](#step-4-get-burp-suite-ready)
- [Step 5: Configure Burp Suite](#step-5-configure-burp-suite)
- [Step 6: Create a Desktop Shortcut](#step-6-create-a-desktop-shortcut)
- [Troubleshooting](#troubleshooting)

### Step 1: Install Java

Before getting started, let's install Java.

For this demo, we're using **OpenJDK 21**. BurpLoader supports Java 11–26, but we recommend **Java 21 or 25** for Burp Suite compatibility.

Open your terminal and run:

```bash
sudo apt update
sudo apt install openjdk-21-jdk -y
```

### Step 2: Verify Java Installation

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

### Step 3: Download BurpLoader

Now it's time to download BurpLoader!

You can download it directly from the GitHub release: [**Download burp-loader.jar**](https://github.com/Esther7171/BurpSuite-Toolkit/releases/tag/v1.0)

Or, if you're lazy like me and prefer the terminal, use `wget` to download it directly.
```bash
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
```

For this demonstration, I'm using the **Desktop** directory to keep everything organized and easy to access. Feel free to save BurpLoader and your Burp Suite installer anywhere you prefer.

### Step 4: Get Burp Suite Ready

Now for the main ingredient: **Burp Suite!** 🍔

You can download Burp Suite directly from the official PortSwigger website. I've also added the latest stable release to this repository's GitHub Releases, so if you're lazy like me and don't want to hunt for download links, I've got you covered!

#### Option 1: Download from GitHub Releases

You can download the version included in this repository directly using `wget`:

```bash
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar
```

I'll try to keep the repository updated with stable releases whenever possible, so you don't have to search for them manually.

#### Option 2: Download from the Official Website

Prefer downloading directly from the source? No problem!

Visit the official [PortSwigger Burp Suite Releases](https://portswigger.net/burp/releases) page to find the latest available version.

**Important: Select the JAR format**

When downloading Burp Suite, make sure to select `JAR` from the platform dropdown before clicking the Download button.

<div align="center">
  <img alt="Select JAR format from PortSwigger download options" src="https://github.com/user-attachments/assets/93c5e8d0-87e8-4a50-9aa7-b5e4b1738e84">
</div>

The JAR package runs across supported operating systems using a compatible Java runtime. We'll use the same download format for `Windows`, `Ubuntu`, `Kali Linux` and `macOS`.

### Step 5: Configure Burp Suite

Now that everything is downloaded, let's get Burp Suite up and running!

#### 1. Locate Burp Suite

If both BurpLoader and Burp Suite are saved in the same folder, BurpLoader should automatically detect Burp Suite and display the **Ready to Start** status.

<div align="center">
  <img alt="BurpLoader ready to start interface" src="https://github.com/user-attachments/assets/c387240d-8a69-41a4-b880-5ea544b4c8f2">
</div>

If BurpLoader cannot find Burp Suite, simply click the `Browse` button and manually locate your downloaded Burp Suite JAR file.

> **Tip:** If you opened BurpLoader before downloading Burp Suite, simply restart BurpLoader after downloading it.

#### 2. Launch Burp Suite

Once Burp Suite is detected, click the `Run` button to launch the application.

Be patient! The first startup may take a little longer than usual. Give it a moment to initialize.

*If a JRE warning appears, simply ignore it and continue with the setup.*

<div align="center">
  <img alt="BurpLoader application launch" src="https://github.com/user-attachments/assets/a3ab4cfa-c617-4fa5-a8c6-2cb8f7a7532a">
</div>

#### 3. Accept the Terms and Conditions

When Burp Suite starts for the first time, you'll be presented with the Terms and Conditions.

Read through them and accept the terms to continue.

<div align="center">
  <img alt="Burp Suite terms and conditions" src="https://github.com/user-attachments/assets/fb2e97f8-bb74-421f-8112-ae3e62eb76c9">
</div>

#### 4. Select Burp Suite Professional

On the next screen, select **Continue with Professional**.

<div align="center">
  <img alt="Continue with Burp Suite Professional" src="https://github.com/user-attachments/assets/5ae8923f-19b2-45a8-be33-58293224edb3">
</div>

#### 5. Copy The License From Loader Past in Burpsuite like this and click on next

<div align="center">
  <img width="1775" height="912" alt="image" src="https://github.com/user-attachments/assets/e44a9923-8921-4e92-a85b-1389e7f3b0ad" />
</div>


#### 6. Select Manual Activation

Click on **Manual activation** to proceed with the manual activation process.

<div align="center">
  <img alt="Burp Suite manual activation" src="https://github.com/user-attachments/assets/d88aee9f-9ccc-4b45-898e-882e7958af82">
</div>

#### 7. Copy The Request from Burpsuite paste In bruploader:

<div align="center">
  <img width="1790" height="906" alt="image" src="https://github.com/user-attachments/assets/8a905018-8ec2-415a-bddd-dfd1c00ecad9" />
</div>

#### 8. Copy The Copy Response from burploader Paste in Burpsuite and click Next:

<div align="center">
  <img width="1746" height="929" alt="image" src="https://github.com/user-attachments/assets/bfa7c13c-221f-4046-ada7-c5899cf59660" />
</div>

#### That it ur License is activated enojy ur burpsuit:

<div align="center"> <img width="1774" height="933" alt="image" src="https://github.com/user-attachments/assets/76b9d431-f143-4f00-8c78-de27085edae8" /> </div>

That's it! Your Burp Suite setup is complete. To launch it again, simply run BurpLoader using the command below:

```
java -jar burp-loader.jar
```

Once BurpLoader opens, click **Run** and Burp Suite will launch. 

### Step 6. Create a Desktop Shortcut

I know it's annoying to launch BurpLoader and open the terminal every time you want to use Burp Suite. So, let's make life easier by creating a desktop shortcut!

#### 1. Create the Shortcut
 
In BurpLoader, click the **Create Shortcut** button to add Burp Suite to your Ubuntu application launcher.

<div align="center"> <img alt="Create Burp Suite desktop shortcut" src="https://github.com/user-attachments/assets/88c1ad4c-8749-4e65-8583-ecf327c233ef"> </div>

#### 2. Confirm the Shortcut

If Burp Suite has already been configured, click **Yes** when prompted to confirm the shortcut creation.

> **Note:** Creating a shortcut before completing the configuration may cause it to open an unconfigured Burp Suite instance.

<div align="center"> <img alt="Confirm Burp Suite shortcut creation" src="https://github.com/user-attachments/assets/a160b5b4-7db3-4ddc-9123-dc55bcacd73a"> </div>

#### 3. Find Burp Suite in the Application Launcher

Once the shortcut is created, Burp Suite will appear in your Ubuntu application launcher.

<div align="center"> <img alt="Burp Suite in Ubuntu application launcher" src="https://github.com/user-attachments/assets/788a84ba-d5c1-45a0-8dc8-ef5584545ae4"> </div>


#### 4. Pin Burp Suite to the Dock

For even quicker access, right-click the Burp Suite icon in the application launcher and select **Add to Favorites** (or the equivalent pin option in your Ubuntu version).

<div align="center"> <img alt="Pin Burp Suite to Ubuntu dock" src="https://github.com/user-attachments/assets/01ef18c2-509b-44e0-93ca-e12af2a6ee08"> </div>

#### That's it! You're all set. You can now launch Burp Suite directly from your Ubuntu dock without manually opening the terminal or BurpLoader every time.

Happy Hacking! 🚀
