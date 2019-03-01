# (DRAFT) Electrum KeepKey Integration for Ubuntu (Linux)

To setup KeepKey integration with Electrum, here are the following steps:  
  
I. Install Electrum  
  
Open Terminal.  
Enter following command: sudo apt-get install python-qt4 python-pip  
Enter following command: sudo pip install https://download.electrum.org/2.6.4/Electrum-2.6.4.tar.gz

II. Install KeepKey Client

Open Terminal.  
Enter following command: sudo apt-get install python-dev python-setuptools cython libusb-1.0.0-dev libudev-dev git  
Enter following command: sudo pip install keepkey

III. Ubuntu (Linux) Permissions

Open Terminal.  
Enter following command: sudo wget https://raw.githubusercontent.com/keepkey/chrome-proxy/master/51-KeepKey.rules  
Enter following command: sudo mv 51-KeepKey.rules /lib/udev/rules.d/  
Reboot.