Nov 2, 2018  
A personal note about how to install __Ubuntu 18.04__ on __MacBookPro High Sierra 10.3(Mid2015)__.  

# Motivation
It is a waste of time to do the tricky way install linux-based software on mac, sometimes it work temporary, most of time it bites.  
Some essential tools running on Ubuntu not OS, for a poor EE student:
* __NS3__ - I know a tricky way to install on Mac
* __theano__ - most likely there is a way to fit into Mac now, but not 4 years ago
* __ROS__ - the huge monster cost too much, virtual machine would not help
* __GNU Radio__ - no reason it would fit into Mac OS
* __CNTK__ - look when Microsoft are willing to fit it for Mac OS, likely coming soon. 

# Reference
[How to get Ubuntu 18.04 (Linux) on Mac OS X / macOS (Dual Boot)](https://www.youtube.com/watch?v=kRgKlcm1XPI), a youtube link highly recommend.        
Some essential link:        
*   [Bootable Drive Maker for Mac](https://github.com/GregoryConrad/BootableDriveMaker/releases/download/v7.0/Bootable.Drive.Maker.dmg)       
*   Command to run in Ubuntu to install rEFInd      
``` shell
    sudo add-apt-repository ppa:rodsmith/refind && sudo apt update && sudo apt install refind && sudo refind-mkdefault
```



# Several aspects not mentioned in the video
1. ```Disk utility``` cannot patrition the new Ubuntu partition request, error like __not enough APFS space to continue ...__  
Solution: leave some space used, e.g. 250G disk is partited as 210G for macOS, all remaining 40G for Ubuntu. Such greedy-case would not work, while 210G + 38G(for Ubuntu) + 2G plan would do.  
2.  It is must to follow the video way - at the begining of loading USB installer, __jump into live demo fist then do the install__, other way like directly install would fail when formatting allocated disk. Besides, once it fail, you have to go back to mac OS, use Disk Utility to format the Ubuntu disk again.