# ardupilotInstallUbuntu

prerequirements install:

sudo apt-get update
sudo apt-get install git
sudo apt-get install gitk git-gui  (optional?)
sudo apt install python3
sudo ln -s /usr/bin/python3 /usr/bin/python
sudo apt install python-dev-is-python3
sudo apt-get install gcc-arm-none-eabi
sudo apt-get install g++-arm-linux-gnueabihf
sudo apt install make -y

git thingy:

git clone https://github.com/ArduPilot/ardupilot.git
git checkout ArduCopter-stable
git submodule update --init --recursive

build example:

alias waf="$PWD/modules/waf/waf-light"
waf configure --board=F4BY
waf 
