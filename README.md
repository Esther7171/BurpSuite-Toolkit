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

<img width="1581" height="723" alt="image" src="https://github.com/user-attachments/assets/5c5e6b0f-2379-4845-aafd-db9c7d1ea165" />




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
