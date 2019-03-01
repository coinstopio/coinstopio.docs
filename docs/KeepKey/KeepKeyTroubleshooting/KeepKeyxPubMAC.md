# (DRAFT) Obtaining xPub On OS X

To obtain xpub on KeepKey with OS X El Capitan, do the following:  
  
_**I. Install pip**_  
  
- Open Terminal.  
- Enter following command - sudo easy_install pip

_**II. Install Cython**_  
  
- Open Terminal.

- Enter following command - sudo pip install cython  
  
_**III. Install KeepKey Python Client**_  
  
- Open Terminal.  
- Enter following command - sudo -H pip install  HTTPS://GITHUB.COM/KEEPKEY/PYTHON-KEEPKEY/ARCHIVE/MASTER.ZIP

_**IV. Retrieve xpub**_ _**key**_  
  
- Open Terminal.

- Enter following command - keepkeyctl get_public_node -n "44'/0'/0'"

- Enter PIN according to KeepKey screen and placement of numbers in command prompt.