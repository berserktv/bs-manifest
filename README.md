# Berserk manifest

#### Minimalistic Linux distribution that acts as an IPTV Multimedia Center Kodi

---  
##### Build by Yocto Project 

###### for Raspberry Pi Platform
---  


To get the "Berserk" source code you need to have `repo` installed and use it as:

Install the `repo` utility:

```sh
$  mkdir ~/bin
$  curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$  chmod a+x ~/bin/repo
```

Download the "berserk" source:  
(example build v0.2.6 for Raspberry Pi 3B and 3B+, branch rocko)  

```sh
$  PATH=${PATH}:~/bin
$  mkdir torvin
$  cd torvin
$  repo init -u https://github.com/berserktv/bs-manifest -m raspberry/rocko/torvin-0.2.6.xml
$  repo sync
```

At the end of the commands you have every metadata you need to start work with.  

To start a "berserk" image build:  

```sh
$  cd torvin
$  ./shell.sh
$  bitbake berserk-image
```

You can use any directory to host your build. 

The source code is checked out at `berserktv/berserk`.

## Contributing

To contribute to this layer you should send the patches for review to the mailing list:  
    mailto: berserktv@yandex.ru  

Source code manifest:  
    https://github.com/berserktv/bs-manufest  

Source code berserk:  
    https://github.com/berserktv/berserk  
    
