# AV Linux 
Install AV Linux (AVL-MXE-2020.12.03-xfce4-amd64): http://www.bandshed.net/avlinux/

* `sudo apt-get update`
* `sudo apt-get upgrade`
* `sudo apt-get dist-upgrade`
* `sudo apt-get install emacs`
* `sudo apt-get install python3-pip`
* `sudo pip3 install setuptools`

# SuperCollider
Build from source: https://github.com/supercollider/supercollider/blob/develop/README_LINUX.md

* `sudo apt-get install build-essential cmake libjack-jackd2-dev libsndfile1-dev libfftw3-dev libxt-dev libavahi-client-dev`

- follow supercollider linux build from source doc
- terminal, cd <space>, mkdir supercollider_build, cd supercollider_build
- git clone
- cd SuperCollider
- make build dir 
- cmake with type release and native option 
- make -j5 
- sudo make install
