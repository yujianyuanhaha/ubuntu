# downgrade package
`apt-get install PACKAGE_NAME version`

# install .deb
`dpkg -i PACKAGE_NAME.deb`

# add path
e.g. `export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/lib/x86_64-linux-gnu`, and check by `echo $LD_LIBRARY_PATH`, while __delete__ with TODO.


# ln
softlink, nothing but shortlink.  
``` bash
 ln -s passwd passwd-so
 ```