# beelink-ndimonitor-how-to-install
A How-to setup a Beelink AP34 with Ubuntu and Sienna-TV´s NDIMonitor

## Ubuntu Installation:
* Download ubuntu ISO at least 18.04.2 (it´s supporting the beelink eMMC storage out of the box) from ubuntu.com
* Create a bootable stick from the ISO (you can use etcher: https://www.balena.io/etcher/)
* Boot the beelink while pressing F7 and select the USB stick.
* Install ubuntu to Beelink, choose default Ubuntu.
* At the screen where you enter username, remember to tick: Log in automatically

## Ubuntu setup:
* In upper right corner press arrow down
* Omenu press the settings button 
* Go to power section and set: 
  * Dim screen: off
  * Blank Screen: never
  * Automatic Suspend: off

## Install NDI-monitor:
* Download NDI-monitor and place it in your home folder.
* Open terminal (press ctrl-alt-t)
```
sudo apt-get install libsdl2-2.0 curl -y
cd 'NDI Monitor’
chmod +x NDIMon*
./NDIMonitor_License_Manager
```
* Enter your licence key
You can now try the monitor:
```
./NDIMonitor
```
After testing type:
```
gnome-session-properties
```
* Press "Add"
* Name: NDIMonitor
* Press browse and and double-click on the NDIMonitor file.
* Save

### Reboot and hopefully you now have a working NDIMonitor.
