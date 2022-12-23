# Ardupilot Build On Ubuntu

prerequirements install:<br>
<br>
sudo apt-get update <br>
sudo apt-get install git<br>
sudo apt-get install gitk git-gui  (optional?)<br>
sudo apt install python3<br>
sudo ln -s /usr/bin/python3 /usr/bin/python<br>
sudo apt install python-dev-is-python3<br>
python -m pip install empy<br>
sudo apt-get install gcc-arm-none-eabi<br>
sudo apt-get install g++-arm-linux-gnueabihf<br>
sudo apt install make -y<br>

<br>
git thingy:<br>
<br>
git clone https://github.com/ArduPilot/ardupilot.git<br>
git checkout ArduCopter-stable<br>
git submodule update --init --recursive<br>
<br>
build example:<br>
<br>
alias waf="$PWD/modules/waf/waf-light"<br>
waf configure --board=F4BY<br>
waf copter<br>
<br>
