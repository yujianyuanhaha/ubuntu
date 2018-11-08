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
*   [Bootable Drive Maker for Mac](https://github.com/GregoryConrad/BootableDriveMaker/releases/download/v7.0/Bootable.Drive.Maker.dmg) (it would fail sometimes, start over)       
*   Command to run in Ubuntu to install rEFInd      
``` shell
    sudo add-apt-repository ppa:rodsmith/refind && sudo apt update && sudo apt install refind && sudo refind-mkdefault
```



# Several aspects not mentioned in the video
1. ```Disk utility``` cannot patrition the new Ubuntu partition request, error like __not enough APFS space to continue ...__  
Solution: leave some space used, e.g. 250G disk is partited as 210G for macOS, all remaining 40G for Ubuntu. Such greedy-case would not work, while 210G + 38G(for Ubuntu) + 2G plan would do.  
2.  It is must to follow the video way - at the begining of loading USB installer, __jump into live demo fist then do the install__, other way like directly install would fail when formatting allocated disk. Besides, once it fail, you have to go back to mac OS, use Disk Utility to format the Ubuntu disk again.

3. When do several partition, e.g. a UBUNTU & a SWAP, it suggest to __split one by one__, else it would fail, saying no enough APFS space while actually there is enough.



4. __uninstall ubuntu__ and __Parittion Combination__.
Be aware when uninstall ubuntu, it is far more complicate than easy-format-and-combine. When I follow some [blog](), it cannot goes through by serveral commands. Since I got the time machine backup, I directly format the whole disk to erase the partition.   
Several bugs I met and solution:
    1. Launch __Boot Camp__ app to reload the available size, when the available space size of diskutility does not match the system information.
    2. If you have not set EFI yet, and you want to revert. A esier way is format the partition disk as Mac Journal, and then click "-" under the map to revert.

4. __Format the disk__ .Once you got all set and still want to use the USB stick, you need the macOS app [SD Card Formatter](https://www.sdcard.org/downloads/formatter_4/eula_mac/index.html) to format the stick, the disk utility woud not work.


5. __macOS Sierra High+ Ubuntu16.04__
Would not work, it could boot into chip sys, but crash when do the installation, say error "interal error".