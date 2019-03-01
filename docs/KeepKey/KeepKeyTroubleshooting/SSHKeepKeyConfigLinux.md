# (DRAFT) SSH KeepKey Configuration With Ubuntu (Linux)

To setup KeepKey SSH Login with Ubuntu (Linux), here are the following steps:  
  
I. Install Python-Dev Python-Tools Libusb-1.0.0-dev Libudev-dev and Git.  
Open Terminal.  
Enter following command: sudo apt-get install python-dev python-setuptools libusb-1.0-0-dev libudev-dev git

II. Install Pip.  
Open Terminal.  
Enter following command: sudo easy_install pip

Install KeepKey Python Client.  
Open Terminal.  
Enter following command: sudo pip install https://github.com/keepkey/python-keepkey/archive/master.zip

III. Install Trezor Python Client.  
Open Terminal.  
Enter following command: sudo pip install trezor

IV. Install Trezor_Agent SSH.  
Open Terminal.  
Enter following command: sudo pip install trezor_agent

V. Generate SSH Public Key using trezor-agent.  
Open Terminal.  
Enter following command: trezor-agent user@sshserver (user - user name and sshserver is server name)  
Enter PIN.  
  
VI. Copy ECDSA key into Authorized Keys on SSH Server  
Log into SSH Server  
Copy ECDSA Key that was created from the previous step  
Paste into ~/.ssh/authorized_keys file on your SSH Server  
VII. Login into SSH Server using your KeepKey  
Open Terminal  
Enter following command - trezor-agent -c user@sshserver (user - user name and sshserver is server name)  
Enter PIN  
Hold KeepKey button for 2 seconds to authenticate