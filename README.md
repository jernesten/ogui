# ogui - Ocalmfuse Graphical User Interface
Linux Graphical user interface for GDrive ocamlfuse build in python3 - CC-BY-NC-SA - License

After days of confinement caused by the appearance of the "damn virus". I have decided to spend my time learning to program in python. A way to get something good out of the situation, and to maintain sanity despite being locked up for so long.
It is a small application that serves as a graphical interface to control the Ocalmfuse program write by Astrada and also shared in github.
https://github.com/astrada/google-drive-ocamlfuse

The application allows you to manage more than one google drive account, according to the parameters defined for the ocamlfuse program.

Sorry if the code is not as fancy as python could allow, but this is my first python app. However I am open to suggestions if someone thinks they know how to improve it.

![ogui sample](https://github.com/jernesten/ogui/blob/master/images/ogui-sample.png "OGUI Image Sample")

# How to use OGUI

 Ogui is just a GUI for ocamlfuse.
 So in order to be able tou mount your google drive account you need to install first the Astrada's program.
 
## Install ocamlfuse by Astrada in your Linux system

### Ubuntu systems and derivates 

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

### For other systems or other installation options

For installing inother systems, please go to [Astrada's ocamlfuse github](https://github.com/astrada/google-drive-ocamlfuse) and follow instructions


For other installation options, please refer to his [wiki](https://github.com/astrada/google-drive-ocamlfuse/wiki/Installation).

## Clone or download OGUI

```
git clone https://github.com/jernesten/ogui.git
```
- Start OGUI
- Add a new google drive account
- Mount it
- Look for it in your file manager

# Acknowledgments

Thank you very much to my friends Úrsula and Jorge without whom I would probably still be stuck at some point in development.
	

