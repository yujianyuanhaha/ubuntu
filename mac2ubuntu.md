# Bugs
## memory-consuming chrome
Ubuntu18.04 on MacbookPro Mid2015 would stuck for minitues for some reason. High likely the __chrome eaily eat up all 8G memory__. Prefer command as much as you can.  
Several Solution from [refer](https://askubuntu.com/questions/817966/google-chrome-will-take-up-my-memory-to-the-point-where-it-causes-my-computer-to/817995)
    * increase RAM  
    * increase swap by [gparted]()  
    * frequent `Shift+Esc` to kill tab  
    * [chrome plugin Great Susper](https://chrome.google.com/webstore/detail/the-great-suspender/klbibkeccnjlkjkiokjodocebajanakg?hl=en)



# Hardware

## Screenshot

## workspace


## Sleep
Do __super+L__ to lock before close the lid, else the system would crash.




## Bluetooth
Would fail on Airpod and Beats, use a wired one.

## USB to Gigabyte Internet Port
TODO

# Backup
TODO

# 

# VPN
Pulse still works on Ubuntu 18.04, refer to [VPN virginia tech](https://vt4help.service-now.com/sp?id=kb_article&sys_id=d5496fca0f8b4200d3254b9ce1050ee5#linux) for more.
1. download newest version ` ps-pulse-linux-9.0r2.0-b819-ubuntu-debian-64-bit-installer.deb
`
2. install by `sudo dpkg -i PACKAGE_NAME`
3. install dependency as prompts
4. launch GUI, follow steps as [VPN virginia tech](https://vt4help.service-now.com/sp?id=kb_article&sys_id=d5496fca0f8b4200d3254b9ce1050ee5#linux).


# SSH and ARC access
[ssh setup tutorial](https://github.com/yujianyuanhaha/blog/blob/master/source/_posts/tutorial/ssh.md)


# Copy and Paste in terminal
Still works
normal  | Ubuntu 
------------ |-------------
Ctr+C| Ctr+Shift+C
Ctr+V| Ctr+Shift+V


# App map
Mac OS | Ubuntu
------------ | -------------
Microsoft Office | (Online) Google Doc
Evernote | Online
iCloud (Notes, Reminder, Calender, Photos, Drive) | Online, Keep Google, __Tasks Google iOS__
Quick Pen Drawings of Notes/Evernote | Keep Google
Professional Slides Drawing | Draw Google/ Libre Draw
Google Drive | Online
iThoughtX (MindMap) | Online Coogle/__Google Task__
Mail | Chrome plugin Checker Plus/ Online/ Thunderbird
Github | GitKraken
cmd+shift+ G of Finder | Commands `grep` `find`/ cmd
Screenshoot | -
Pulse Secure (VPN) | Pulse Secure .deb
Preview | Document Viewer/ Foxit
TexMaker/ Latex | Online overleaf/ TexMaker/ VS Code
LatexIt | LibreMath+ TexMath plugin
Matlab | ssh Matlab on ARC 

# shortkey map

## System

function | Mac OS | Ubuntu 
------------ |------------ | -------------
search & app & overview | super+Shift+S | super
quick terminal | - | Alt + F2
terminal | - | Ctr+Alt+T(erminal)
desktop | _swap away_ |super+D(estop)
Apps | _F4_ | super+A(pp)
Alt App | - | super + Tab/ Alt + Tab
Alt Tab in SubPage | - | Alt + Tab
Alt Window in App| - | __super + `__
snap window | - | __super + arrow__

[Reference](https://itsfoss.com/ubuntu-shortcuts/)




## Chrome
function | Mac OS | Ubuntu 
------------ |------------ | -------------
history | cmd + Y | Ctr + H
download | cmd + shift + J | Ctr + J



## Spyder default
function  | key
------------ |-------------
Comment/ UnComment | Ctr + 1
Run | F5
Begin Debug| Ctr+F5
Continue | Ctr + F10
Stop | Ctr + Shift + F12
Step | Ctr + F11
Step into | Ctr + F11
Step out | Ctr + Shift + F11
ident | Tab
unindent | Tab + Shift
add block comment | __Ctr+4__
remove block comment | __Ctr+5__
 


## VS Code default
function  | key
------------ |-------------
New window | Ctr + Shift + N
Open Folder | Ctr+K Ctr+O