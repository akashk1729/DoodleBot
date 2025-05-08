## Setting up your Raspberry Pi 4 wireless.

## 1.Material needed

Here you will learn about Raspberry Pi, what you need to use it and how to configure it.

It is usually necessary to use a keyboard ⌨️, a mouse 🖱️ and a monitor 🖥️ to start using Raspberry Pi for your projects. In this guide we will use the most current version of software as of April 2021. And we will only need a laptop 💻, a Raspberry Pi 4 and its power supply.

There are several Raspberry Pi models. Raspberry Pi 4 Model B is the newest, fastest and easiest to use.

![raspberry-pi](https://user-images.githubusercontent.com/79243784/116725445-86bb8180-a9a7-11eb-9737-83d1cb6611f7.png)

Raspberry Pi 4 comes with 2GB, 4GB, or 8GB of RAM. For most educational purposes, hobbyist maker projects, and desktop use, 2GB is sufficient.
 
As I mentioned what we will need is:
 
* Laptop
* Raspberry Pi 4
* Power supply (Preferably buy the official source together with your Raspberry so as not to have any problems, if you don't have much experience [USB-C Power Supply](https://www.raspberrypi.org/products/type-c-power-supply/))
* Smartphone with Mobile Hotspot function
* Micro SD card
 
A very important part before starting is the selection of a Micro SD card, since we will load the operating system on it, in the figures we can see a micro SD memory where we will take into account the black boxes, this symbol indicates us in the table the classifications of current micro SD cards, it is very important to note that the minimum speed that should be used in a Raspberry Pi is 10 Mb / sec and with a capacity of at least 8GB.
 
It will be noticed in the speed of ignition and the execution of some tasks. It is not so important to have the most expensive SD to have a better performance in the Raspberry, but having a good card can extend its useful life since the Raspberry Pi makes heavy use of the cards and ends up damaged which means buying another one.

![sd](https://user-images.githubusercontent.com/79243784/116725537-9fc43280-a9a7-11eb-9cbf-9b0a78fb80ec.jpg)

![SDFAQ-UHS-2](https://user-images.githubusercontent.com/79243784/116725548-a357b980-a9a7-11eb-9001-005e23f84b4d.jpg)


Many vendors include SD cards for Raspberry Pi that are already configured with the Raspberry Pi operating system and ready to use with kits but they usually come with NOOBS.
 
NOOBS is an application that facilitates the installation of various Linux distributions on the small computer.
 
NOOBS makes Internet access unnecessary during the installation, and we will only have to download NOOBS and unzip it on an SD card of at least 4 GB capacity. Doing so will give us the option to install solutions such as Raspbian, Arch Linux, RaspBMC, the newly released Pidora or OpenELEC without problems. The installation will later allow us to start our Raspberry Pi normally with that new distribution, but NOOBS will remain memory resident and we can access this application whenever we want by pressing the Shift key during the startup process.
 
As a personal preference, I think it is better to buy a memory from a brand like SanDisk and do the installation as shown below.


**Note: You should avoid disconnecting the power source without having the Raspberry turned off, this can damage the memory at the moment and everything would be lost, nor by formatting the memory could it be used again**

## 2.Installing Raspberry Pi OS via Raspberry Pi Imager
 
Using Raspberry Pi Imager is the easiest way to install the operating system
Raspberry Pi on your SD card. ** Note: Raspberry Pi OS is not the only operating system that
can be installed. ** The steps outlined below can be used to
install other operating systems compatible with Raspberry Pi, but the initial configuration
when you turn on it will be different. For more information on other operating systems visit [installing operating system images](https://www.raspberrypi.org/documentation/installation/installing-images/README.md).
To Download and run the Raspberry Pi Imager visit the [Raspberry Pi downloads page](https://www.raspberrypi.org/downloads).
Click on the link for the Raspberry Pi Imager that matches your operating system.

When the download is complete, click on it to launch the installer.
When you start the installer, your operating system may try to block its execution (In that case you have to click ** more info ** within the installer window to continue and click **Run anyway**).
 
Once Raspberry Pi imager is installed
 
1. Insert your SD card into the SD card slot of the computer or computer
laptop.
 
2. In Raspberry Pi Imager, select the operating system you want to install ❶ and
the SD card on which you want to install it ❷ (See Figure).
**Note: You will need to be connected to the Internet the first time for Raspberry Pi Imager to download the operating system of your choice. That operating system will be stored for future offline use. Being online for later uses means that the Raspberry Pi Imager will always provide you with the latest version**

![imager1 5](https://user-images.githubusercontent.com/79243784/116725672-dc902980-a9a7-11eb-8a63-256c3c9a9bdb.png)

In case of having a card with another previous operating system or with some files, we can use the Raspberry Pi Imager to format and leave it as new.
 
We will select "CHOOSE OS" and we will click on Erase, we will return to the main window we will select "CHOOSE SD CARD" and we will select our card, "WRITE" is enabled, we will click, a window will appear where we will confirm and ready we have our card ready to be overwrite with Raspberry OS.

![ERASEMEDIUM](https://user-images.githubusercontent.com/79243784/116725748-fd587f00-a9a7-11eb-9cb9-372214212224.png)

To play with the advanced options that will allow us to access our Raspberry remotely, you must press the key sequence:
 
"Ctrl-Shift-X"
 
That will display a window in which we will select the "Enable SSH" box, it will also request that we enter a password for the pi user, which is the default user in Raspberry pi, usually the password is Raspberry for this user, but with this option you can enter the one you like.

![enablesshraspberry](https://user-images.githubusercontent.com/79243784/116725836-1a8d4d80-a9a8-11eb-9d7c-fad1703848c3.png)

Going down further in this window we can find the "configure wifi" box where we enter the network name and password, as I mentioned before we will use a smartphone, which will function as a modem (in my case I use a Samsung phone, which has the option to Hotspot, when a device connects to my phone it appears in connected devices and when I click on the device it gives me the IP address), later we will talk about the IP, as the last one in this window at the end it allows us to choose the country in the that we are for some language configurations, at the end we will click on save and we will return to the main window.

![WIFIPASSWORDMEDIUM](https://user-images.githubusercontent.com/79243784/116725892-2da01d80-a9a8-11eb-8e96-ab92b30edb88.png)

Now we will select the operating system by clicking on "CHOOSE OS". For those who are starting with a Raspberri, it is recommended to use the first option, and for more experienced users the second allows us to choose the lite version that is recommended for some specific projects.

![chooseOSMEDIUM](https://user-images.githubusercontent.com/79243784/116726028-588a7180-a9a8-11eb-8354-54f56439f030.png)

Now we will click on "CHOOSE SD CARD" to select our card, by clicking we will return to the main window. The "WRITE" button is enabled, we click and a message will appear requesting confirmation of the writing of the operating system.

![sdchooseMEDIUM](https://user-images.githubusercontent.com/79243784/116726065-64763380-a9a8-11eb-9a53-4b80c71dc335.png)

At the end of the writing of the operating system on the card, the following window will appear with this we will have the micro SD memory ready to connect it to our Raspberry Pi.

![succesOSwritemedium](https://user-images.githubusercontent.com/79243784/116726093-6dff9b80-a9a8-11eb-8851-94d40f4c5eac.png)

To connect the sd card it is very easy at the bottom of our Raspberry you can find the slot where it is placed.

![pi-sd](https://user-images.githubusercontent.com/79243784/116726123-77890380-a9a8-11eb-8a17-7006dd378c2c.png)

Finally we will connect the power source first to our Raspberry and then to a plug. **In case of connecting first to the plug and then to the Raspberry we could cause small shorts that could affect the useful life of our card**.

![pi-power](https://user-images.githubusercontent.com/79243784/116726143-7e177b00-a9a8-11eb-99f8-b25aeff90cd3.png)

## 3.SSH Windows
 
You can access the command line of a Raspberry Pi remotely from another computer or device on the same network using SSH. The Raspberry Pi will act as a remote device: you can connect using a client on another machine. You only have command line access, not the full desktop environment.
For a full remote desktop, see VNC and its installation guide [How to Remote Desktop to your Raspberry Pi with VNC Viewer](https://www.raspberrypi.org/documentation/remote-access/vnc/).

**Note: In the latest versions of Raspberry Pi OS, only VNC needs to be enabled, so it is not necessary to install the server as the VNC link shows**
 
With the previous steps we have already enabled SSH in our Raspberry now we will access for the first time to start working.
 
Previously we mentioned about the IP in case of not having the hotspot function you can check other ways to obtain them in [Raspberry IP](https://www.raspberrypi.org/documentation/remote-access/ip-address.md)
 
We will need to install Putty, it is an SSH client developed for Windows. PuTTY is open source software that is available with source code. To download visit [Putty](https://www.putty.org/)
 
When we install Putty, the following will appear and we have to select what is shown marked in the image.

![puttymediumintal](https://user-images.githubusercontent.com/79243784/116726205-95eeff00-a9a8-11eb-888f-6ccdc74bf818.png)

When we start, the following window will appear, where we enter the IP of our Raspberry. Then we will click on open.
It will send us an alert message in which we will click Yes.

![puttyMEDIUM](https://user-images.githubusercontent.com/79243784/116726263-a69f7500-a9a8-11eb-877a-61de557b3cc3.png)

After clicking yes, the window where the user will be entered will appear if the password was not changed and the factory user comes as pi user and the password that we established in the previous steps as raspberry.

![loginuserMEDIUM](https://user-images.githubusercontent.com/79243784/116726299-b3bc6400-a9a8-11eb-9af8-af93e9c0e0f4.png)

After entering, our user will ask us for the password.

![passworduserMEDIUM](https://user-images.githubusercontent.com/79243784/116726317-b9b24500-a9a8-11eb-90e6-8d9ab857772d.png)

Once the password is entered, it will show us the window as shown in the figure and we will have full access to the Shell of our Raspberry. Now we are going to configure it to get access to the desktop.

![inMEDIUM](https://user-images.githubusercontent.com/79243784/116726393-d0f13280-a9a8-11eb-96a5-2c61ba9c3781.png)


## 4.VNC
 
Sometimes it is not convenient to work directly on the Raspberry Pi. Maybe you would like to work on it from another remote control device like your laptop. VNC is a graphical desktop sharing system that allows you to remotely control the desktop interface of a computer (with VNC Server) from another computer or mobile device (with VNC Viewer). VNC Viewer transmits keyboard and mouse or touch events to the VNC Server and receives updates on the screen in return. You will see the Raspberry Pi desktop within a window on your computer or mobile device. You can control it as if you were working on the Raspberry Pi itself. In short it is very similar to using TeamViewer.
From Putty we enter the terminal of our Raspberry. Once in our terminal we enter the command:
 
 
```
sudo raspi-config
```

![sudoraspiconfigMEDIUM](https://user-images.githubusercontent.com/79243784/116726482-f41be200-a9a8-11eb-9bd7-fdca2796dffc.png)


We will go to the next window and select option 3 "Interface Options".

![SUDOINTERFACEOPTIONESMEDIUM](https://user-images.githubusercontent.com/79243784/116726512-0269fe00-a9a9-11eb-82fb-fde953578709.png)

Now the following options will appear, we will select VNC.

![VNCMEDIUM](https://user-images.githubusercontent.com/79243784/116726547-0f86ed00-a9a9-11eb-9e95-eedd4d13adf6.png)

We will confirm that we want to enable the VNC server.

![VNCyesMEDIUM](https://user-images.githubusercontent.com/79243784/116726568-16156480-a9a9-11eb-84b7-574234f2e0af.png)

We will return to the sudo raspi-config menu, now we will select "Display Options"

![DisplaYMEDIUM](https://user-images.githubusercontent.com/79243784/116726595-1e6d9f80-a9a9-11eb-84ea-64ac2ed54e24.png)

Now we will select D1 Resolution. To configure a resolution that does not have problems with our team.

![RESOLUTIONmedium](https://user-images.githubusercontent.com/79243784/116726655-32190600-a9a9-11eb-8b1c-56fb42bbb700.png)


We will select DMT Mode 85. The 1280 x 720 resolution is compatible with most of the current equipment, in case it does not look very good on your equipment try using some of the other options with lower resolution.

![DTMresolutionMEDIUM](https://user-images.githubusercontent.com/79243784/116726729-4bba4d80-a9a9-11eb-8915-5e58d4d98941.png)

![RESOLUTIONokmediUM](https://user-images.githubusercontent.com/79243784/116726754-55dc4c00-a9a9-11eb-97ba-cd637bc9c66b.png)


When confirming, it will ask us if we want to restart, my recommendation is the "YES" option. After restarting, our Raspberry will be ready to enter the Desktop for the first time.

![YESrebootMedium](https://user-images.githubusercontent.com/79243784/116726902-81f7cd00-a9a9-11eb-96dc-383bbc8f8908.png)

We have to install VNC on our computer, to download visit [VNC Download](https://www.realvnc.com/es/connect/download/viewer/), once installed you can open the program, enter at the top the IP of our Raspberry.

![VNCmedium2](https://user-images.githubusercontent.com/79243784/116726967-96d46080-a9a9-11eb-85cf-00ba1f1bfa29.png)

The following window will appear where we enter the username and password of our Raspberry Pi. We will accept and it will show us the Raspberry Pi desktop.

![inicioVNCmedium](https://user-images.githubusercontent.com/79243784/116726987-9c31ab00-a9a9-11eb-82c1-cd3b402d6302.png)

Once logged in from our Windows computer we will be able to see the desktop of our Raspberry Pi remotely, we will click on ok in the warning window and we will proceed to follow the following steps:
 
When you start your Raspberry Pi for the first time, the Welcome to Raspberry Pi application will appear and guide you through the initial setup. Click Next to start the configuration.

![inicioRaspMEDIUM](https://user-images.githubusercontent.com/79243784/119272320-f7cb0f00-bbca-11eb-911a-9cf0b180c3e2.png)

![NEXTmediuminicio](https://user-images.githubusercontent.com/79243784/116727522-4dd0dc00-a9aa-11eb-8f97-e13f60915045.png)

Set your country, language, and time zone, then click Next again.

![countriraspbMEDIUM](https://user-images.githubusercontent.com/79243784/116727082-b8354c80-a9a9-11eb-80f4-93d92d54022d.png)

It will give us the option to enter a new password for your Raspberry Pi, it is not necessary to change the password, from the factory Raspberry has a pi user and raspberry password, the change is only for security. and click Next.

![SETPASSWORDmedium](https://user-images.githubusercontent.com/79243784/116727123-c71bff00-a9a9-11eb-95f9-d4734d3a0522.png)

It will give us the option to eliminate the black borders on a screen, as we are using a remote server we cannot see the borders that would normally appear if we connected our Raspberry via HDMI so we will omit this option and click Next.

![setupscreenMEDIUM](https://user-images.githubusercontent.com/79243784/116727147-cd11e000-a9a9-11eb-85de-854635d46cc1.png)

It will allow us to connect to another wireless network by selecting its name, entering the password (**Changing the network while you are in SSH or VNC will automatically close the application, the Raspberries have a dynamic IP that changes each new network that connects , you will have to enter the new IP of the network to access remotely again**), we will continue with the configuration by clicking Next.

![NETWORKmedium](https://user-images.githubusercontent.com/79243784/116727183-d4d18480-a9a9-11eb-911a-eaf52de16e9d.png)

The option to update will appear, it is best to click Next and let the wizard look for updates to the Raspberry Pi operating system and install them (this may take a little time).

![updateMEDIUM](https://user-images.githubusercontent.com/79243784/116727213-ddc25600-a9a9-11eb-9055-ab4fb34cf48d.png)

If the update was executed successfully, the following window will appear, in case it fails, it is best to follow the instructions and then, by Putty in SSH, enter the commands:
 
1. sudo apt update
2. sudo apt full-upgrade
 
If everything went well, we will click Ok.

![readyMEDIUM](https://user-images.githubusercontent.com/79243784/116727267-f16dbc80-a9a9-11eb-85fc-ca4a39865bf6.png)

We will click Restart to finish the configuration.
 **Note: You will only need to reboot if necessary to complete an update.**

![REBOOTAGAINmedium](https://user-images.githubusercontent.com/79243784/116727306-fdf21500-a9a9-11eb-9145-cc3199afab0c.png)

With these steps completed, our Raspberry is ready for us to use for our projects. Now you can enter your Raspberry using any of the previous methods and create with this tool.
 
If you want to know more about how to start Raspberry for the first time, visit its official page [Setting up Raspberry](https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up)
 
In case you are interested, you can review the guide on [how to install Visual Studio Code and Git on Raspberry Pi](https://github.com/fullmakeralchemist/gitvscoderaspberry).

