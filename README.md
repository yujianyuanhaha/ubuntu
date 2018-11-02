Ubuntu Notes
OS: 18.04

Essential command tools:
1. vim
2. git  

Optional command tools:
1. openssh-server, for set up ssh.

For these tool, mostly install by ```sudo apt-get install SOFTWARENAME``` would work.


My personal recommened apps:
1. Chrome, all-in-one, it got many plugins work as desktop-apps:
    * ad-blocker
    * pocket
    * evernote
    * translator
    * pdf viewer
    * google input tools (works for Chinese)
    * check plus for gmail
2. GitKraken, mostly used to trace codes
3. Anaconda
    * Spyder
    * Visual Studio Codes, with plugins
        * markdown preview
        * live server 



Some optional but useful apps:
1. Sublime, lightweight editor
2. Foxit reader, used to annote pdf
3. Dropbox, driver
4. Whatever, evernote client



# Wifi of eduroam
There need some special setup to connect to ```eduroam``` wifi, take Vriginia Tech as example. Follow the [offical setup](https://vtluug.org/wiki/Virginia_Tech_Wifi) by vtluug. It is bit too long, to be breif, follow the picture below:  
![](wifi.png)  
while for CA certificate: Select ```/path/to/GlobalSign_Root_CA_-_R3.pem``` via the file picke



# Anaconda
## install
Follow offical guide [Installing on Linux](http://docs.anaconda.com/anaconda/install/linux/).
1. download [Anaconda3-5.3.0-Linux-x86_64.sh](https://www.anaconda.com/download/#download) file, this is for python 3.5.
2. in terminal , run ```bash Anaconda3-5.3.0-Linux-x86_64.sh```.
3. do ``` source ~/.bashrc```, and then launch ```anaconda-navigator```.

## bugs
the bugs seem appear on Ubuntu 18.04  
When prompt to ask __install VS Code__, it always answer __no internet connection__, just let it go. You can install VS Code later when finished install Anaconda.  
When install VS Code in the Anaconda Navigator GUI, it would stuck some how, Ctr+C stop it, type ```sudo apt --fix-broken install```, and install it from Anaconda Navigator again.  


# GitKaren
Version 4.0.6



## install
* Ubuntu Software app
* download the deb file, then ```dpkg -i gitkraken-amd64-18.04.deb ```

## bugs
The window would not show up after the dancing octupus, you could look into the logs by command ```gitkraken``` in termianl to launch,refer to [failed to load module "canberra-gtk-module"](https://askubuntu.com/questions/342202/failed-to-load-module-canberra-gtk-module-but-already-installed) and [Gitkraken won't open gui
](https://askubuntu.com/questions/1050338/gitkraken-wont-open-gui), install missing tools by ```sudo apt install libcanberra-gtk-module libcanberra-gtk3-module``` as well as ```sudo apt install libgnome-keyring0```, then __restart__.
