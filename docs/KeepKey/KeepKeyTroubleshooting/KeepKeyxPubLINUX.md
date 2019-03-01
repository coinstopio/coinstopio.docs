# (DRAFT) Obtaining xPub On Ubuntu (Linux)

To obtain xpub on KeepKey with Ubuntu, complete the following steps:  
  
**_I. Install pip_**  
  
- Open Terminal.  
- Enter following command - sudo easy_install pip

_**II. Install Cython**_  
  
- Open Terminal.  
- Enter following command - sudo pip install cython

_**III. Install Libsub**_  
  
- Open Terminal.  
- Enter following command - sudo pip install libusb-1.0.0-dev

_**IV. Install KeepKey Python Client**_  
  
- Open Terminal.  
- Enter following command - sudo pip install  HTTPS://GITHUB.COM/KEEPKEY/PYTHON-KEEPKEY/ARCHIVE/MASTER.ZIP

  
_**V. Retrieve xpub key**_  
  
- Open Terminal.  
- Enter following command - keepkeyctl get_public_node -n "44'/0'/0'"  
- Enter PIN according to KeepKey screen and placement of numbers in command prompt