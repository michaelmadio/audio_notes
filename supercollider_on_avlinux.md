Tested on 2020/12/07

# AV Linux 
Install AV Linux (AVL-MXE-2020.12.03-xfce4-amd64): http://www.bandshed.net/avlinux/

* `sudo apt-get update`
* `sudo apt-get upgrade`
* `sudo apt-get dist-upgrade`

# SuperCollider
Build from source: https://github.com/supercollider/supercollider/blob/develop/README_LINUX.md

* `sudo apt-get install build-essential cmake libjack-jackd2-dev libsndfile1-dev libfftw3-dev libxt-dev libavahi-client-dev`
* `sudo apt-get install qt5-default qt5-qmake qttools5-dev qttools5-dev-tools qtdeclarative5-dev qtwebengine5-dev libqt5svg5-dev libqt5websockets5-dev`
* `sudo apt-get install emacs`
* `cd `
* `mkdir supercollider_build; cd supercollider_build`
* `git clone --recurse-submodules https://github.com/SuperCollider/SuperCollider.git`
* `cd SuperCollider`
* `mkdir build; cd build`
* `cmake -DCMAKE_BUILD_TYPE=Release -DNATIVE=ON ..`
* `make`
* `sudo make install`
* `sudo ldconfig`

# SuperCollider SC3 Plugins
Build from source: https://github.com/supercollider/sc3-plugins

* `cd ~/supercollider_build`
* `git clone --recursive https://github.com/supercollider/sc3-plugins.git`
* `cd sc3-plugins`
* `mkdir build; cd build`
* `cmake -DCMAKE_BUILD_TYPE=Release -DNATIVE=ON ..`
* `make`*
* `sudo make install`
* `sudo ldconfig`

# FoxDot
https://foxdot.org/
* `sudo apt-get install python3-pip`
* `sudo pip3 install setuptools`
* `sudo apt-get install python3-tk`
* `sudo pip3 install FoxDot`

# Atom Editor
https://atom.io/
https://flight-manual.atom.io/getting-started/sections/installing-atom/#platform-linux
* `wget -qO - https://packagecloud.io/AtomEditor/atom/gpgkey | sudo apt-key add -`
* `sudo sh -c 'echo "deb [arch=amd64] https://packagecloud.io/AtomEditor/atom/any/ any main" > /etc/apt/sources.list.d/atom.list'`
* `sudo apt-get update`
* `sudo apt-get install atom`
