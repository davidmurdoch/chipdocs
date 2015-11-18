# Using DERP
If you've used a desktop or laptop computer before, DERP should be pretty familiar. There are menus, icons to click, right-click for more stuff, keyboard shortcuts, applications to run, and settings to set. CHIP is small, so we keep DERP simple. Almost everything can be accessed from the **Computer Things** menu: settings, launching apps, and access to files. There's also a few convenient functions in the top right **system tray.** Keep reading this document to find out more about how to use and configure DERP on CHIP!

## Settings and Configuration
Most of the settings for the computer and for the desktop can be set using the apps in the "Computer Things" menu. Select the appropriate app from either the Settings Menu or the Settings Manager.

![Screenshot of GUI showing where to change WiFi settings](images/screen_settingsmenu.jpg)

![Screenshot of GUI showing where to change WiFi settings](images/screen_settingsmgr.jpg)

### WiFi

A connection to a WiFi network is easily made using the WiFi icon the top right system tray. Just select a network to initiate a connection. If you need a password, you'll be prompted for it.

![Select a wireless connection access point](images/screen_wifisettings.jpg)

If you need more control and information over your network connection, use the Settings->Network Connections panel to show your connections. Double click on a connection to bring up the connection editor:

![Network connection editor](images/screen_networksettings.jpg)

### Bluetooth
Bluetooth device setup can be accessed using the Bluetooth icon in the top right system tray.

![Bluetooth settings menu](images/screen_btsettings.jpg)

When you begin a connection, you'll be guided through the necessary steps to connect to your device. For example, when you pair with a keyboard, you'll be prompted for a code to enter to ensure a unique connection. Once you have paired a device, future connections will usually be automatic when the devices are in range and powered up.

![Bluetooth settings menu](images/screen_btsetup01.jpg)

You can manage, and also connect to, your devices using the the Bluetooth Devices panel, accessed from the Bluetooth system tray:

![Bluetooth devices panel](images/screen_btdevices.jpg)

### Sound
By default, sound output comes from the built-in connector, served by the "sunxi codec" driver. If you want to change the volume, you can use the volume control in the top right system tray:

![Desktop volume control](images/screen_volumectl.jpg)

Or, open the Audio Mixer in the Multimedia category:

![Open Audio Mixer app in Multimedia category](images/screen_audiomixermenu.jpg)

where you can select the "Playback" category to change the volume.

![Control panel for sound](images/screen_audiosettings03.jpg)

If you don't see that control, just click on the "Select Controls" button and enable all controls:

![Enable all controls for audio mixer](images/screen_audiosettings02.jpg)

### Display
Use the Settings->Display control panel to adjust the monitor's resolution and rotation settings:

If you want to customize the desktop image, icons, colors, and fonts, there are two different panels. The Appearance panel lets you select a theme to make instant changes for several properties.

![Change monitor settings with the Display control panel](images/screen_desktopsettings04.jpg)

The Desktop panel lets you customize images and colors, along with the behavior of menus.

![Change desktop look with Desktop panel](images/screen_desktopsettings01.jpg)

### Time and Date
Set the Time with the Orage Globaltime panel. This can be found in Accessories->Orage Globaltime or in Office->Orage Globaltime. Simply click the time to bring up the preferences panel. You can quickly view the date from the Orage Calendar in the Office menu.

![Orage Globaltime is used to set the time and date](images/screencap_timesettings.jpg)

### Mouse Sensitivity
Screenshot and description of using GUI desktop to change Mouse Sensitivity settings.

![Screenshot of GUI showing where to change mouse sensitivity](images/screencap_mousesettings.jpg)

## Launching Installed Apps
DERP comes prepackaged with many open-source applications to get you started. It's easy to launch an application. 
You can select an application from the "Computer Things!" menu and select an app from the categories:

![Screenshot of GUI launching apps](images/screen_appfinder01.jpg)

Or, for more control, launch the Application Finder in Accessories, where you can use the search bar and easily navigate among the categories:

![Screenshot of GUI launching apps](images/screen_appfinder02.jpg)

Below are some of the applications that come pre-installed with CHIP:

### AbiWord
AbiWord is a fully featured word processor. You can learn more at [The AbiWord website](http://www.abiword.org)

![AbiWord can process words.](images/appscreen_abiword.jpg)

### Web Browser
Ice Weasel is a Debian Linux version of the Firefox browser. The browser is largely the same as Firefox, but has a different name for the sake of trademark protection by the Mozilla corporation. More information is at the [Debian website](https://wiki.debian.org/Iceweasel) and in this [stack exchange thread](http://unix.stackexchange.com/questions/44215/is-there-any-advantage-of-using-iceweasel-and-firefox).

![Browse the web with IceWeasel](images/appscreen_webbrowser.jpg)

### Video Player
CHIP plays video! Use the built-in Mplayer to open and play videos.

![Mplayer plays video](images/appscreen_videoplayer.jpg)

### Terminal (commandline)
The life blood of linux. If there's something you can't do on the desktop, or you want to automate tasks, or access different hardware settings using nothing but a keyboard and text, you'll open up Terminal.

![Terminal does even more computer things](images/appscreen_terminal.jpg)

## Install and Update Software

### Synaptic Package Manager
Launch the Synaptic Package Manager to find and install new software. 
This is a graphical interface to the `apt-get` command and will install software for DERP and other debain-based systems.

![Install software with Synaptic](images/appscreen_synaptic.jpg)

### Auto Update
CHIP will automatically look for any updates and alert you if updates are available for your existing software and DERP operating system.

### apt-get

If you are using the commandline, you will use `apt-get` to install and update new software.

If you are new to apt, some important commands to know:
```shell
apt-get update
```shell
updates the information from repositories, so any installs you make with `install` will be the latest package
```shell
apt-get upgrade
```
upgrades any installed packages.
```
apt-get install <name of package>
```
to install a package and any of its dependencies.
```shell
apt-get remove <name of package>
```
will remove a package and any dependencies not used by other packages
```shell
apt-get purge  <name of package>
```
will remove a package and any dependencies not used by other packages along with all settings data
```shell
apt-cache search <search terms>
```
will search through the package repositories for names and descriptions that include your search term.

### Chrome-based Update Interface