# TP-wn722n-

TP-LINK wn722n v2/3 make error fix in Kali Linux Kernel v 5.18.0-kali2-amd64


cd Desktop
git clone https://github.com/IceM4nn/mirrorscript-v2
cd mirrorscript-v2
sudo python3 mirrorscript-v2.py


sudo apt update
sudo apt upgrade
sudo apt dist-upgrade
sudo apt upgrade        //to make sure everthing upgraded//
sudo reboot
sudo apt install bc
sudo apt-get install build-essential 
sudo apt-get install libelf-dev 
cd Desktop
git clone https://github.com/KanuX-14/rtl8188eus.git
cd rtl8188eus
sudo -i
echo "blacklist r8188eu" > "/etc/modprobe.d/realtek.conf"
exit
sudo reboot
cd Desktop
cd rtl8188eus
sh -c "$(curl -fsSL https://raw.githubusercontent.com/KanuX-14/rtl8188eus/v5.3.9/build.sh)"


To enable Monitor mode and test packet injection:

sudo ifconfig wlan0 down
sudo airmon-ng check kill
sudo iwconfig wlan0 mode monitor
sudo ifconfig wlan0 up
ifconfig
iwconfig                             
sudo aireplay-ng --test wlan0
