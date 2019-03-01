# KeepKey Wallet Not Recognised By Linux

If after installing the KeepKey wallet on a Linux machine and it has not recognised the KeepKey device, please follow the steps detailed below:

1.  Open **t****erminal**.
2.  Enter the following command:  
      
    wget https://raw.githubusercontent.com/keepkey/udev-rules/master/51-usb-keepkey.rules
3.  Enter the following **command**:  
      
    sudo mv 51-usb-keepkey.rules /etc/udev/rules.d/
4.  **Reboot**  
      
    Linux Commands:  
      
    sudo - execute command as superuser with password  
    wget - download files from the web  
    mv - move files  
      
    # KeepKey: Your Personal Hardware Security Module  
    # http://www.keepkey.com/  
    # Put this file in /lib/udev/rules.d  
      
    SUBSYSTEM=="usb", ATTR{idVendor}=="2b24", ATTR{idProduct}=="0001", MODE="0666", GROUP="dialout", SYMLINK+="keepkey%n"  
    KERNEL=="hidraw*", ATTRS{idVendor}=="2b24", ATTRS{idProduct}=="0001", MODE="0666", GROUP="dialout"