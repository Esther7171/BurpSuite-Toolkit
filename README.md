# BurpSuite-Toolkit

## About the Project

## Features

## Supported Platforms

## Tested Environments

## Installation Guide

### 1. Windows Installation
[Coming Soon]

### 2. Linux Installation
 




#### Ubuntu Setup
Step-by-step instructions


How to setup BurpSuit professional on Ubuntu as im using `Ubuntu 26.04.1 LTS`

Let 1st install java on it u can download any for demo im using java 21

```
sudo apt update
sudo apt install openjdk-21-jdk -y
```
Let check if it install properly
```
java -version
javac -version
```

<img width="710" height="195" alt="image" src="https://github.com/user-attachments/assets/87d2143f-0716-4d8c-9d21-11966cd19cda" />

Now Time to Dowload the burploader u can download directly from github release by clicking here -> https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar


Or if ur guys are lazy like me just download with wget as i open the desktop to direct to save everthing here to easy display and setup gude u guys can save burpload and burpsuit anyhere u want 

```sh
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/v1.0/burp-loader.jar
```

Now Main inderdient Burpsuit u can download it from offical link or i already added current latest and stable release in github release and ill upload ever stable version so guy just lzy like dont have to worry about it

```
wget https://github.com/Esther7171/BurpSuite-Toolkit/releases/download/Professional_and_Community/burpsuite_desktop_v2026.10.1.jar
```

So if u dont trust me u can download the offical version burpsuit from here or if forgot to push anylatest version to release as im am lazy u know so u can donload it from here

So where is link of offical download page its in the app so u dont have to find it manully
Let laucnh loader 1st to start u have to use below cmd.

```
java -jar burp-loader.jar
```

U can see a little prompt will apper 

<img width="1105" height="631" alt="image" src="https://github.com/user-attachments/assets/49554001-deb8-48a9-83b4-0b931252ddcf" />

click on offical Page it will redirect u to offical release page if u still have finding trouble https://portswigger.net/burp/releases 

photo 1 
<img width="1162" height="380" alt="image" src="https://github.com/user-attachments/assets/867162c6-319a-4fb9-a134-cc18240ccf55" />

photo 2

<img width="1161" height="387" alt="image" src="https://github.com/user-attachments/assets/93c5e8d0-87e8-4a50-9aa7-b5e4b1738e84" />

Now u meet all condition Let start configuring burpsuit:

As u have both loader and burpsuit in same folder it will say Read to start, If ur Burploader cant able to find burpsuit please ur browse button to locate ur burpsuit or if u lauch burploader 1st and download burpsuit later relauch please or just run no matter.

Photo 1:
<img width="1581" height="723" alt="image" src="https://github.com/user-attachments/assets/5c5e6b0f-2379-4845-aafd-db9c7d1ea165" />

Photo 2:

<img width="1077" height="601" alt="image" src="https://github.com/user-attachments/assets/7546ebe0-8bc9-43a9-bf02-8c9bfc040bf0" />

After clicking run be patient at 1st burpsuit need little time to open , AND ignore jre warning

<img width="1061" height="603" alt="image" src="https://github.com/user-attachments/assets/a3ab4cfa-c617-4fa5-a8c6-2cb8f7a7532a" />

Accept the Terms and condition

<img width="593" height="531" alt="image" src="https://github.com/user-attachments/assets/fb2e97f8-bb74-421f-8112-ae3e62eb76c9" />

Click On Continue With Professional 

<img width="608" height="693" alt="image" src="https://github.com/user-attachments/assets/5ae8923f-19b2-45a8-be33-58293224edb3" />

Copy The License From Loader Past in Burpsuite like this and click on next:

<img width="1775" height="912" alt="image" src="https://github.com/user-attachments/assets/e44a9923-8921-4e92-a85b-1389e7f3b0ad" />

Then Click On Manully activtion

<img width="602" height="499" alt="image" src="https://github.com/user-attachments/assets/d88aee9f-9ccc-4b45-898e-882e7958af82" />

Copy The Request from Burpsuite paste In bruploader

<img width="1790" height="906" alt="image" src="https://github.com/user-attachments/assets/8a905018-8ec2-415a-bddd-dfd1c00ecad9" />

Copy The Copy Response from burploader Paste in Burpsuite and click Next

<img width="1746" height="929" alt="image" src="https://github.com/user-attachments/assets/bfa7c13c-221f-4046-ada7-c5899cf59660" />

That it ur License is activated enojy ur burpsuit

<img width="1774" height="933" alt="image" src="https://github.com/user-attachments/assets/76b9d431-f143-4f00-8c78-de27085edae8" />

to create a shortcut , click on create shorcut button
<img width="1075" height="769" alt="image" src="https://github.com/user-attachments/assets/88c1ad4c-8749-4e65-8583-ecf327c233ef" />

> If u create shortcut without activating burpsuit it will open unconfig burp, if u configed it click yes

<img width="602" height="186" alt="image" src="https://github.com/user-attachments/assets/2eae3ef6-94ea-43a3-b740-2528289d944a" />

Your burpsuite pro will be added to ur application launcher

<img width="1608" height="592" alt="image" src="https://github.com/user-attachments/assets/788a84ba-d5c1-45a0-8dc8-ef5584545ae4" />

by right clicking it u can pin it to dock and close rest of ur burploader and terminal with single click ur burpsuit pro will be ready

<img width="1918" height="1049" alt="image" src="https://github.com/user-attachments/assets/01ef18c2-509b-44e0-93ca-e12af2a6ee08" />






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
