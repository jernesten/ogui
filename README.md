<p>
        <img src="https://github.com/jernesten/ogui/raw/master/images/ogui.png" style="padding-top:25px" align="left">
        <h1>OGUI - GDrive Ocalmfuse GUI</h1>
</p>
  

Linux Graphical User interface for GDrive ocamlfuse made with python3 - v. 1.4.21 Beta.

**CC-BY-NC-SA - License**

----

OGUI is a small application that serves as a graphical interface to control the Ocalmfuse program write by Astrada and also shared in github.
https://github.com/astrada/google-drive-ocamlfuse

The application allows you to manage more than one google drive account, according to the parameters defined for the ocamlfuse program.

Sorry if the code is not as fancy as python could allow, but this is my first python app. However I am open to suggestions if someone thinks they know how to improve it.

![ogui sample](https://github.com/jernesten/ogui/blob/master/images/ogui-sample.png "OGUI Image Sample")

## :inbox_tray: Installation

 OGUI is just a GUI for google-drive-ocamlfuse.
 So in order to be able to mount your google drive account you need to install first the Astrada's program.
 
### Debian, Ubuntu systems and derivates

#### The easy way

- Clone or [download](https://github.com/jernesten/ogui-installer/archive/master.zip)
```
git clone https://github.com/jernesten/ogui-installer
```
- extract if needed
- go to the extracted folder
- execute script
```
chmod +x ogui-installer
sh ogui-installer
```
[More information.](https://github.com/jernesten/ogui-installer)

#### The less easy way

For ubuntu systems and derivates Astrada has uploaded .deb packages into his PPA. In order to install it, use the commands below:
```
sudo add-apt-repository ppa:alessandro-strada/ppa
sudo apt-get update
sudo apt-get install google-drive-ocamlfuse
```
Depending on your Linux distribution you may need to run before
```
sudo apt-get install software-properties-common
```
Clone or [download](https://github.com/jernesten/ogui/archive/master.zip)
```
cd ~/
git clone https://github.com/jernesten/ogui
```
Install dependencies
```
sudo apt-get install git python3 python3-tk
```
Extract if needed and copy the extracted folder into ~/.local/share
```
chmod +x ~/ogui/py/ogui
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
Move or copy de desktop file into ~/.local/share/applications directory to have the ogui option in your applications menu (this action is useless for openbox menu)
```
chmod +x ~/ogui/ogui.desktop
cp ~/ogui/ogui.desktop ~/.local/share/applications/ogui.desktop
```

### For other systems or other installation options

#### Installing gdrive-ocalmfuse
For installing in other systems, please go to [Astrada's ocamlfuse github](https://github.com/astrada/google-drive-ocamlfuse) and follow instructions

For other installation options, please refer to his [wiki](https://github.com/astrada/google-drive-ocamlfuse/wiki/Installation).

#### Installing OGUI

The same as for Debian/Ubuntu systems.
Even the script should be useful.

## :wrench: How to use

**Buttons:**

- "New:" --> Add a new google drive account
- ![Mount](https://github.com/jernesten/ogui/blob/master/images/mount.png) --> Mounts the Drive
- ![Unmount](https://github.com/jernesten/ogui/blob/master/images/unmount.png) --> Unmounts the Drive
- ![Edit](https://github.com/jernesten/ogui/blob/master/images/edit.png) --> Edit the Drive account
- ![Delete](https://github.com/jernesten/ogui/blob/master/images/delete.png) --> Delete the Drive account

**So:**
- Start OGUI
- Add a new google drive account
- Mount it
- Look for it in your file manager


:rainbow:
---

:smile:Thank you very much to my friends Úrsula and Jorge without whom I would probably still be stuck at some point in development.:wink:

---
---

