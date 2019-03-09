# (DRAFT) SSH KeepKey Configuration With OS X

To setup KeepKey SSH Login with OS X El Capitan, here are the following steps:  
  
I. Install Pip.  
Open Terminal.  
Enter following command: sudo easy_install pip

II. Install KeepKey Python Client.  
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
  
VI. Copy ECDSA key into Authorized Keys on SSH Server.  
Log into SSH Server.  
Copy ECDSA Key that was created from the previous step.  
Paste into ~/.ssh/authorized_keys file on your SSH Server  
  
VII. Login into SSH Server using your KeepKey.  
Open Terminal.  
Enter following command: trezor-agent -c user@sshserver (user - user name and sshserver is server name)  
Enter PIN.  
Hold KeepKey button for 2 seconds to authenticate.