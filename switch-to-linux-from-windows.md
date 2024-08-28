# A Guide on how best to switch from Windows to Linux for daily use
-by diam0ndkiller

Like everyone in the Linux community, I always see videos of people trying the switch to Linux but not having a single straight-forward guide at hand. A lot of guides on the internet are good, but they don't work especially well with each other.
So I decided to write my own one, in order to make it easier for you guys.
## 0. What is Linux
In order to understand this guide or in order to even consider switching, you first need to understand what Linux even is.

Linux is an operating system for your computer. Much like the more-known alternatives Windows and MacOS, it is responsible for providing an interface and applications for you to use your PC. The difference however is, that, contrary to Windows and MacOS, Linux is not backed by a big company. On one hand that means that you don't have official support hotlines, but on the other hand it means that the possibilities on Linux are not limited by a money-making construct, but rather by a free community.

Most of the time people switch to Linux, because they either
- don't like the look and feel of their own previous operating system or (way more often)
- dislike the direction the large company backing their system is going regarding data collection or accounts for example.

But most people get discouraged very fast by the large amount of distributions available. Like I said, Linux is a community-driven project. But that also means, that everyone can take their own approach to it.

You see, Linux itself is not an operating system, it is a base for multiple Linux-like operating systems, called distros. There are hundreds if not thousands of distros around the internet, and A LOT of guides do a bad to horrible job of helping you choose. But don't go just now. I'm not going to make that mistake. Instead, I'll and recommend ONE SINGLE distro to you:

![[linuxmint-logo-mono.svg]]

## 1. Linux Mint
The Linux Mint operating system is a Linux distribution that is targeted to beginners. But it has a few perks that make me use it till to day.

The project is driven by a team of developers and is, like most other projects in the Linux space, developed **free** and **open-source** (FOSS). That means, that everyone who has the knowledge and is interested can look into and modify the source code, to fix bugs, add feature requests or just try to understand it.

As of writing this article, Linux Mint just released it's version 22, codenamed Wilma. To download it, visit [[https://linuxmint.com/download.php]]. There, you will be greeted with three different "Editions" of Linux Mint:

- The "Cinnamon Edition":
  This is the most popular version of Linux Mint, which I recommend to most beginners too. It includes a graphical user interface (GUI) that looks and feels like Windows out of the box. However but it can be customized in a lot of ways to work differently.
- The "XFCE Edition":
  This edition ships with a different graphical user interface called XFCE. It is a bit older and lacks some modern features, but is more lightweight and more customizable.
- And finally: The "MATE Edition":
  MATE is similar to XFCE, but it is even more lightweight and even older. I wouldn't recommend it to most users.

All of these versions feature the same base system, but with a different **Desktop Environment** built on top of it. Desktop Environments (or short: DEs) are a part of your graphical user interface. They are responsible for displaying your Taskbar(s) (Panels), your windows and your desktop icons along with other things. In this guide I recommend you use the Cinnamon Desktop Environment, like said before.

You can go ahead and click the "Download" button right now. It will take you to a page of multiple other links. If you scroll down a bit, you will find the "Download Mirrors" section. This is again a result of the community-driven nature of Linux Mint. There is not one big server where you can download the system. Instead, there are multiple small ones, hosted mostly by universities and other organisations, that host the same files for all. Choose a location that is close to your home and click the link. Your download should start now. You can continue reading this post while it runs.

Like promised I'd like to point out some things which make me use Linux Mint to this day.
1. **Stability:** In contrast to some other more advanced Linux users who use more experimental distributions, I like to stay on Linux Mint because I can just be sure that my system stays operational, whatever updates or packages I install.
2. **Software Support:** Linux Mint is based on Ubuntu, a very popular distro for both servers and PCs. Because of that Mint offers software support for a lot of programs that are maybe more niche, because they have been ported to the more-known Ubuntu system. That also includes graphcis drivers for NVIDIA, which can be hard to find on some other distributions.
3. **Community:** From both a beginner's and a advanced's perspective the Linux Mint community is a great place to be. The forums make the life easier for you and let me help other people. And the developers in this community care a lot about the ideas of the users.
4. **Customizability:** Even though there are other options that can be more customized, all three editions of Linux Mint (Cinnamon, XFCE and MATE) can be customized a lot which makes them a solid base for almost everyone without having to install a lot of tools.

## 2. Booting and Media
In order to install an operating system on your PC, you need to create a "bootable media". This is just a USB stick that behaves as if it were a hard disk or SSD inside your computer and that contains an operating system.

In order to create it, I recommend you use a tool called **Ventoy**. Download it from [[https://ventoy.net/en/download.html]]. Click the windows.zip link and in the list click the windows.zip link again to download it. Open the downloaded archive and extract it to your downloads folder by using the "Extract All" button at the top of the window. If you don't get there automatically, navigate to your downloads and open the folder where you extracted Ventoy. Inside you will find a file called `Ventoy2Disk`.

Now insert a USB stick. It can be any stick you want, just note that
**EVERYTHING ON THAT STICK WILL BE DELETED**
when you install Ventoy to it. Afterwards you are able to copy everything back onto it but make sure to have a backup.

After inserting your stick, launch the `Ventoy2Disk` program by double-clicking it. You will be greeted with a window. On the top, Select the USB stick you want to use. Then just click "Install". Once again:
**ALL YOUR FILES WILL BE REMOVED!**

After you installed Ventoy to your stick, it's as simple as to copy the downloaded `linuxmint-something.iso` file onto your USB stick, which should now be called "Ventoy". Congratulations! You now have a bootable USB stick and you can put as many operating systems or other files on it as you wish.

In order to start the Linux installation, you have to restart your PC. As soon as it starts to turn back on, hit the BIOS key of your PC. BIOS is a basic system that runs before you launch into your operating system. Normally the BIOS key is Escape, F1, F2, F9 or the Delete key. This next part might look a bit sketchy but it is totally right to do. If none of these keys do anything, you can google the BIOS key for your specific device.

I promise you, this is the most complex part of the guide!

You will now be greeted with either a boot menu or a more complex BIOS menu. If you just see a list of different media labelled EFI, SATA, USB or something like that, you entered the boot menu. Use the arrow keys to select the USB entry and hit enter.

If you have a more complex interface with multiple tabs, don't worry! You just entered the BIOS of your computer. You just need to use the arrow keys or in some cases even the mouse to go to the BOOT tab. Now there are three options:

#### 1. Boot override
If you see a "Boot Override" somewhere on screen, navigate to it. Here you will be able to boot from your USB stick like described above.

#### 2. Boot order with multiple rows
If you see a heading called "Boot order" or "Boot priority" and see multiple lines of different names below it, follow these instruction.
1. Navigate to the USB entry.
2. Use the keys shown at the bottom of the screen to move it up to the first position.
3. Search for the "Save and Exit" key on the bottom of your screen and press it.

#### 3. Boot order with a single row
If you see a single column showing e.g. HDD -> SSD -> USB, it means you have a one-line boot priority menu. Just hit SPACE or Enter on it, until USB is at the front position. Now search for the "Save and Exit" key at the bottom of your screen and press it.

If you followed your steps, after some time, you should now see a screen with a Ventoy sign. Perfect! You just booted from your USB stick. You can do these steps on any PC if you want to install Linux from now on. From the shown list, use the arrow keys to select `linuxmint-something.iso`. Hit enter twice and you should finally see a green Linux Mint logo. Congrats, you just started Linux for your first time!

## 3. Live System and Installation
After the system has started, you will see your graphical interface for the first time. Linux Mint supports a system called "Live Session", "Live System", or "Live ISO". That means, that you can test the operating system before installing it. Cool, right? You are in that environment right now. You can try clicking some buttons or icons. Don't worry, you can't break anything. When you are ready, click the CD icon in the top left corner. This will start the installer.

#### Installer Steps
##### 1. Language
First you will get asked for the installation language. Your choice here will set the language of the installer from now on and the language of the entire system after installation.
##### 2. Keyboard Layout
Independently of your language of choice, you can set your keyboard layout. This is VERY IMPORTANT, for if you don't set it correctly, you might not find keys you are searching for. The keyboard layout ensures, that the descriptions on your physical keyboard match what you type on your screen.
##### 2.5. Network
If you didn't connect before and if you don't have a wired connection, you will now be prompted to connect to a WiFi network. Just connect by entering the password for your WiFi like you do on any other device. You could technically work without it but it is required for the next step to work and it will save you some hassle later.
##### 3. Multimedia codecs
Now is the second time you will see results of the free and open source nature of Linux Mint. You will be asked if you want to install **multimedia codecs**. You don't have to understand what that is exactly, just that they are required for some video and audio formats to correctly play. They are entirely in the background, and the only reason that they aren't automatically installed is that they are not in fact free and open source in nature. A default Linux install is per definition totally free and open source, so you need to actively accept this software, in order to install it. Just see this step as a no-brainer. 
**DO CLICK THE CHECKBOX** because you have no reason not to and it will only give you problems later.

For some systems there is also a "Configure Secure Boot" button here. **DO CLICK THAT ONE AS WELL**. You will enter a password which you need in order to install some drivers later.
##### 4. Disk Setup
Now you will be asked to choose where to install Linux Mint to. The recommended option is to just choose "Install alongside Windows". That will keep all your previous files and you can even access them from your Linux Mint install.

If you don't have a lot of storage space, you may have to replace windows by choosing "Replace Windows with Linux Mint" or "Erase Disk and install Linux Mint".
**BE SURE TO BACKUP ANY IMPORTANT FILES BEFORE DOING THAT!**
##### 5. Timezone
Most of the time the installer will ask for your timezone next. Just click near your home on the map and select the right timezone by doing so.
##### 6. User Account
Now you will create the login data for your computer. Enter your name at the top. It should auto-fill the other fields below. Now just enter your password and repeat it. Choose if you want to login automatically or enter your password every time you start your PC.

Click continue for the last time and Linux Mint will start installing to your Computer. You can click through a slide-show showing some programs to keep yourself entertained. Depending on the age of your computer, the install could take from 5 to about 30 minutes. Just let it run and get a snack :)

## 4. Installed System
After the installation has finished you will get a popup asking if you want to continue testing or restart and go into your installed system. If you're ready, just click the "Restart Now" button or just restart your PC from the menu in the bottom left. It will then ask you to remove the USB stick and hit enter. After a reboot you should now be in your ready to use installed Linux Mint system!

#### Welcome Screen
Linux Mint comes with a Welcome Screen that shows you some of the things you can and should do after installation.
##### Desktop Colors
Launch this Program to change the theme and colors of your desktop. You will find your way around it :)
##### System Snapshots
Click this button to launch Timeshift, a program to backup your operating system in case it breaks after an update. Open it and go through the initial setup. Just keep everything as default and finally choose how often you want automatic backups to happen.
**TIMESHIFT DOES NOT BACK UP USER FILES. JUST PROGRAMS AND THE OPERATING SYSTEM!**
Because of that you should be fine creating a snapshot every week or less often. It is just good to have if something doesn't work anymore after an update or something you installed. If that happens, just open Timeshift from the menu and revert back to your snapshot. Then you can go to the forums [[https://forums.linuxmint.com/]] and ask on what to do next. The people there are willing to help if you state your problem kindly and detailed :).
##### Driver Manager
This is a very important tool. Most of the hardware drivers are included in Linux, but sometimes you might have a device which has additional drivers available to make it run better. Most of the time this is with NVIDIA graphics cards and some WiFi devices. Just open the tool and choose the recommended driver. Click "Apply Changes" and enter your password. It will ask you to reboot, but don't do that just now. You have some more stuff to do first.
##### Update Manager
The Update Manager is also a very important component in your system. Use it to keep all the software on your PC, including the operating system itself up-to-date. Open it up right now. You will probably see a popup asking if you want to "Switch to a local mirror". That is again a sign of the de-centralized servers used by Linux Mint. Click "Okay", and then in in the new window Click the "Main" and "Base" buttons and select a server that is near you and has a fast connection. The fastest ones will be at the top. After you did that, click "Update APT cache" at the bottom. You will have a faster server close to you for your packages, which should make updates in the future much more easy. You can close this window now.

Back in the Update Manager, you may be prompted to "Apply the Update" to the Update Manager itself. If so, do it and restart the program. Now just click "Install Updates" in the top bar to install all current updates to get your system up-to-date. After that, reboot your system.
##### Firewall
After rebooting you will find yourself back in the Welcome Screen. Now choose the "Firewall" button to enable security protection from the internet for your PC. This is the last step you need for a fully working and secure operating system.
##### System Settings
You can now go into the system settings and explore your way around. Find something you don't like in some way? It probably has a setting somewhere. Go find it. See it as a fist little challenge!
##### Software Manager
This is an essential part of your system. Other than Windows in previous years, Linux uses an App Store to install programs. In the background, there are different tools and repositories responsible for that, but you only need to worry about the App Store, called "Software Manager". Whenever you need a program, install it through the Software Manager. And only if it's not here, go hunting on the internet.

## 5. Software Compatibility
#### Package types and sources
Linux is the OS of freedom, which also means that there are a lot of ways to do some things. That especially is true for packages, i.e. software installation. In Linux Mint, there are three common *package types* you can use to install software:
##### 1. Debian Packages (system repos)
The first way are the Debian packages. Linux Mint is based on Ubuntu, which is itself based on Debian. Software installed from a Debian package (identified by a `.deb` extension) is located right inside the systems admin directories and has all permissions your user has too. I still like them best though, because the default install location and no permissions mean that they are much easier to use in automated scripts.
###### 1. from the System Repositories
You can get Debian Packages either inside the Software Manager (from the *system repositories*) or from external sources. In the Software Manager, just search the program you want to install and under the install button look for `System Package`. You may have to drop-down and select it.
###### 2. from developer's websites
The second option of where to get `.deb` packages is on developer's websites. This way is similar to how you download software on Windows. Because Ubuntu and Debian are the most used bases of Linux systems, most of the time when you find a download labelled just "Linux", it will be a `.deb` package. Just install it by double-clicking it.
###### 3. from `PPA`s or so called additional repositories
A developer can also choose to provide a custom repository. That is a place on their own server where they host Debian packages. When you find an install guide handling these repositories, use the given instructions in the terminal. The big pro in contrast to normal `.deb` downloads is that external repositories can be updated by the developer and your system Update Manager will automatically pull updates, instead of you having to download any new version.
##### 2. Flatpaks
Flatpak is a newer package format. Its philosophy is that developers should only need to develop one version of an app for Linux, instead of releasing multiple ones for different distributions and versions of them. Flatpak achieves this by being its own program with an app store, that can be installed on most Linux distros. You can find Flatpaks in the Software Manager, just like System Packages.
###### Pros of using Flatpaks:
- You have automatic updates for your apps
- Most of the time you have newer versions of apps, because the developers don't need to wait for the Linux Mint team to release a new version in the System repos.
- You have **permissions** for what your app can access on your system, similar to what Android or iOS would have.
	- Please mind that out of the box there is no graphical way to change these permissions. To do so, please install **Flatseal** from the Software Manager
- You make the job easier for most developers, because they only need to maintain one version of their app for Linux
- Because of that you have more apps available than otherwise.
###### Cons of using Flatpaks:
It might seem that this package format is perfect. But I still prefer System Packages when I can, due to these reasons:
- The apps don't have access to everything out of the box, and I had some issues while I didn't know about the underlying systems.
- The apps are not installed in the default location for apps, but in a sandbox, which makes them hard to work with in scripting.
- They need some tweaks to use the same theme as the rest of your apps.
###### Setup tips for Flatpak:
- Download Flatseal to change permissions for Flatpaks.
- Execute the following commands to use your system's design theme in Flatpak as well:
	- 1. Give Flatpak apps access to your installed themes:
		- `sudo flatpak override --filesystem=$HOME/.themes`
		- `sudo flatpak override --filesystem=$HOME/.icons`
		- `sudo flatpak override --filesystem=/usr/share/themes`
		- `sudo flatpak override --filesystem=/usr/share/icons`
	- 2. Tell Flatpak apps which theme to use (e.g. is `Mint-L` or `Mint-L-Dark-Aqua`)
		- `sudo flatpak override --env=GTK_THEME=Mint-L`
		- `sudo flatpak override --env=ICON_THEME=Mint-L-Dark-Aqua`
##### 3. AppImages
These packages are the equivalent to portable `.exe` applications on Windows. You only have to download one file, double click it and it just runs. To use them like normal applications from your start menu, I would recommend you install an app called "Gear Lever" from the Software Store. It opens when you double click an AppImage file and it lets you quote on quote "install" it to your system, meaning you will find a link to that file in your start menu.
AppImages are widely seen as a bad way to release an app, because they are often very big in size and don't use any permission system, which means that you can accidentally double-click a malicious file from the web.
On the other hand they are also a very simple way for developers to package their apps, because they run almost anywhere. So you will find an `.AppImmage` download link very often on developer's websites. Just be sure that there isn't a native version in the Software Manager before you use the AppImage.

#### Games with Steam
Steam is a good example of a program available in the Software Manager. Just search "steam" and install it. Launch the program and login like normal.
You might have heard that Linux has bad game compatibility. It is true, that most games are not officially built for Linux. But Valve, the company behind Steam, has a fix for that. Go to `Settings > Steam Play > Enable Steam Play for all Titles` to enable Proton, a tool to play almost all games developed for Windows on Linux.

But sadly, the truth is that some popular games aren't supported yet. Mostly due to Anti-Cheat-Systems, some games can't run on Linux. Check [[https://protondb.com]] to see if the games you want to play work with Linux. And if they don't work out of the box, you can also find guides on how to make them work there.
#### Games on EPIC GAMES or GOG using Heroic
For games on the Epic Game Store or GOG there is the Heroic Games Launcher. Just install it from the Software Manager, login with your account and install your games. Although Lutris also has Epic Games and GOG support, I would recommend using Heroic, because it's more specialized.
#### Other games using Lutris
For a lot of other games, there is a program called Lutris. It is a launcher / library for a lot of titles. It has community built installers for a lot of games. If you don't find a game elsewhere, it will probably be here and the community has picked the best way to install it.