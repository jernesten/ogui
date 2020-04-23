# ogui - Google Drive Ocalmfuse Graphical User Interface
Linux Graphical user interface for GDrive ocamlfuse build in python3 - v. 1.4.21 Beta.

CC-BY-NC-SA - License

After days of confinement caused by the appearance of the "damn virus", I have decided to spend my time learning to program in python as a way to get something positive out of the situation, and to maintain my sanity despite being locked up for so long.
It is a small application that serves as a graphical interface to control the Ocalmfuse program write by Astrada and also shared in github.
https://github.com/astrada/google-drive-ocamlfuse

The application allows you to manage more than one google drive account, according to the parameters defined for the ocamlfuse program.

Sorry if the code is not as fancy as python could allow, but this is my first python app. However I am open to suggestions if someone thinks they know how to improve it.

![ogui sample](https://github.com/jernesten/ogui/blob/master/images/ogui-sample.png "OGUI Image Sample")

## Installation

 Ogui is just a GUI for ocamlfuse.
 So in order to be able tou mount your google drive account you need to install first the Astrada's program.
 
### Debian, Ubuntu systems and derivates

#### The easy way (recommended method)

- Clone or download https://github.com/jernesten/ogui-installer
```
git clone https://github.com/jernesten/ogui-installer
```
- extract if needed (if you've download a zip)
- go to the directory
- execute script ('chmod +x ogui-installer' may be needed)
```
sh ogui-installer
```
-choose your option in the menu
```
1. Only install OGUI, GDrive Ocamlfuse is already installed
2. Install both OGUI and GDrive Ocamlfuse
3. Uninstall OGUI
4. Uninstall both OGUI and GDrive Ocamlfuse (It will also remove PPA)
5. Exit            
```
#### The hard way

For ubuntu systems and derivates Astrada has uploaded .deb packages into his PPA. In order to install it, use the commands below:
```
sudo add-apt-repository ppa:alessandro-strada/ppa
sudo apt-get update
sudo apt-get install google-drive-ocamlfuse
```
Depending on your Linux distribution you may need to run before
```
sudo apt-get install software-properties-common
sudo apt-get install python3-software-properties
```
Clone or download https://github.com/jernesten/ogui
```
cd ~/
git clone https://github.com/jernesten/ogui-installer
```
Extract if needed (if you've download a zip) and copy the directory in cp -R ~/ogui ~/.local/share
```
cp -R ~/ogui ~/.local/share
```
Create ogui.desktpo in cp -R ~/ogui ~/.local/share/applications to enable the option in the menu
```
touch  ~/ogui/ogui.desktop
```
Write this inside ~/ogui/ogui.desktop: (change "yourusername" by your actual user name)
```
[Desktop Entry]
Type=Application
Icon=/home/yourusername/.local/share/ogui/images/ogui.png
Name=ogui
GenericName=ogui
Comment=GUI for gdrive ocamlfuse
Categories=Network;
Exec=/home/yourusername/.local/share/ogui/py/ogui
Path=/home/yourusername/.local/share/ogui
Terminal=false
```

### For other systems or other installation options

#### Installing gdrive-ocalmfuse
For installing inother systems, please go to [Astrada's ocamlfuse github](https://github.com/astrada/google-drive-ocamlfuse) and follow instructions

For other installation options, please refer to his [wiki](https://github.com/astrada/google-drive-ocamlfuse/wiki/Installation).

#### Installing OGUI

Clone or download OGUI
```
git clone https://github.com/jernesten/ogui.git
```
Extract if needed (if you've download a zip) and copy the directory in cp -R ~/ogui ~/.local/share
```
cp -R ~/ogui ~/.local/share
```
Create ogui.desktpo in cp -R ~/ogui ~/.local/share/applications to enable the option in the menu
```
touch  ~/ogui/ogui.desktop
```
Write this inside ~/ogui/ogui.desktop: (change "yourusername" by your actual user name)
```
[Desktop Entry]
Type=Application
Icon=/home/yourusername/.local/share/ogui/images/ogui.png
Name=ogui
GenericName=ogui
Comment=GUI for gdrive ocamlfuse
Categories=Network;
Exec=/home/yourusername/.local/share/ogui/py/ogui
Path=/home/yourusername/.local/share/ogui
Terminal=false
```

## Instructions - How to use

**Buttons:**

- ![Mount](https://github.com/jernesten/ogui/blob/master/images/mount.png) --> Mounts the Drive
- ![Unmount](https://github.com/jernesten/ogui/blob/master/images/unmount.png) --> Unmounts the Drive
- ![Edit](https://github.com/jernesten/ogui/blob/master/images/edit.png) --> Edit the Drive account
- ![Delete](https://github.com/jernesten/ogui/blob/master/images/delete.png) --> Delete the Drive account

**So:**
- Start OGUI
- Add a new google drive account
- Mount it
- Look for it in your file manager

## Acknowledgments

Thank you very much to my friends Úrsula and Jorge without whom I would probably still be stuck at some point in development.
	

