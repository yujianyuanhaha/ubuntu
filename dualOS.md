Nov 2, 2018
A personal note about how to install Ubuntu 18.04 on MacBookPro High Sierra 10.3(Mid2015)
# Reference
[How to get Ubuntu 18.04 (Linux) on Mac OS X / macOS (Dual Boot)](https://www.youtube.com/watch?v=kRgKlcm1XPI), a youtube link highly recommend.        
Some essential link:        
*   [Bootable Drive Maker for Mac](https://github.com/GregoryConrad/BootableDriveMaker/releases/download/v7.0/Bootable.Drive.Maker.dmg)       
*   Command to run in Ubuntu to install rEFInd      
``` shell
    sudo add-apt-repository ppa:rodsmith/refind && sudo apt update && sudo apt install refind && sudo refind-mkdefault
```

# Several aspects not mentioned in the video
1. disk utility cannot patrition the new Ubuntu partition reques, error like __not enough APFS space to continue ...__  
Solution: leave some space used, e.g. 250G disk is partited as 210G for macOS, all remaining 40G for Ubuntu.