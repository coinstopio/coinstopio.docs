
# Fix connection issues

If you encounter connection issues when trying to connect your Ledger hardware wallet, try the following solutions one by one.

## Basic: Mac, Windows or Linux

1.  Close other applications

> Ledger apps, crypto wallets, Geth, Parity, Mist, Bitcoin Core, etc

2.  Turn OFF VPN and anti-virus.
3.  Change the USB cable if possible
4.  Try different USB ports.
5.  Restart your computer.
6.  Try another computer.

### If the steps above did not remedy the issue and your problem persists, please view the operating system specific guides below.

## Windows: Advanced

Update USB input device drivers:
    
    1.  Open **Devices and Printers** from Control Panel.
    2.  Double-click **Nano S** and open the **Hardware** tab.
    3.  Select **USB Input Device** and click **Properties**.
    4.  Click **Change Settings**.
    5.  Click the **Driver** tab.
    6.  Click **Update driver** and select automatic driver selection.
    7.  Repeat this for both **USB Input Devices**.
    
>If the issue persists, please try on another operating system to verify that your Ledger Nano S is working properly. This could be on a Mac, Linux or different version of Windows.

## Mac: Advanced

If you're having connection issues on a Mac, you can try giving Ledger Live full disk access:

1.  Open **System Preferences.**
2.  Go to **Security & Privacy**.
3.  In the **Privacy** tab, add Ledger Live to the **Full Disk Access** list.

## Linux: Advanced

On Linux you need to create a set of udev rules to allow device access. Refer to the [Chrome USB API documentation](https://developer.chrome.com/apps/app_usb#caveats) for details. Please follow the instructions below.

### 1. Setup

-   Check if the plugdev group exists by entering the command:  
    
    ```
    cat /etc/group | grep plugdev
    ```
    
#### Follow the steps below if the previous command did not return a result
    1.  **C**reate the **plugdev** group:  
        
        ```
        sudo groupadd plugdev
        ```
        
    2.  Check if you are in the group **plugdev** with the command:
        
        ```
        groups
        ```
        
    3.  If the output does not contain **plugdev**, you are not in the **plugdev** group. Enter the command:
        
        ```
        sudo gpasswd -a <user> plugdev
        ```
        
        **Note**: replace <user> by your username, e.g for user "mike", it would be: **sudo gpasswd -a mike plugdev**.
        
    4.  Logout and login for the change to take effect. To verify you are now in the **plugdev** group, enter:
        
        ```
        groups
        ```
        
        and search for a **plugdev** occurrence. If it's not there, you've missed a step and should restart from step 1.

### 2. Add the udev rules

1.  Enter the following command to automatically add the rules and reload udev:
    
    ```
    wget -q -O - https://raw.githubusercontent.com/LedgerHQ/udev-rules/master/add_udev_rules.sh | sudo bash
    ```
    
2.  Retry connecting your Ledger Nano S with Ledger Live.  
      
    If it's still not working, continue to step 3: troubleshooting.

### 3. Troubleshooting

Try each of the following three options.

-   **OPTION 1**

    **Edit the file **/etc/udev/rules.d/20-hw1.rules** file by adding the **OWNER="<user>"** parameter to each line, where **<user>** is your Linux user name.  
    Then reload the rules as follows:  
    
    ```
    udevadm triggerudevadm control --reload-rules
    ```
    
    Retry the connection with Ledger Live. If it does not work, try the next option.
-   **OPTION 2**  

    Edit the **/etc/udev/rules.d/20-hw1.rules** file and add the following lines:  
    
    ```
    KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0660", GROUP="plugdev", ATTRS{idVendor}=="2c97"
    KERNEL=="hidraw*", SUBSYSTEM=="hidraw", MODE="0660", GROUP="plugdev", ATTRS{idVendor}=="2581"
    ```
    
    Then reload the rules:  
    
    ```
    udevadm triggerudevadm control --reload-rules
    ```
    
    Retry connecting with Ledger Live. If it does not work yet, try the last option.
-   **OPTION 3** 

    If you are on Arch Linux, you can try the following rules:
    
    ```
    /etc/udev/rules.d/20-hw1.rules
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2581", ATTRS{idProduct}=="1b7c", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2581", ATTRS{idProduct}=="2b7c", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2581", ATTRS{idProduct}=="3b7c", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2581", ATTRS{idProduct}=="4b7c", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2581", ATTRS{idProduct}=="1807", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2581", ATTRS{idProduct}=="1808", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2c97", ATTRS{idProduct}=="0000", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2c97", ATTRS{idProduct}=="0001", MODE="0660", TAG+="uaccess", TAG+="udev-acl”
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="2c97", ATTRS{idProduct}=="0004", MODE="0660", TAG+="uaccess", TAG+="udev-acl"
    ```
    
-   Then reload the rules again and retry the connection with Ledger Live:  
    
    ```
    udevadm triggerudevadm control --reload-rules
    ```
    

## iOS and Android

If you're experiencing Bluetooth issues with your Ledger Nano X, please remove the pairing and forget the Ledger Nano X on your phone. Then set up the pairing once again.

### Reset pairings on your Ledger Nano X

1.  Turn on and unlock your Ledger Nano X.
2.  Hold both buttons to access the **Control Center**.
3.  Press both buttons to navigate to the **Security** menu.
4.  Press both buttons to validate **Reset pairings**.
5.  Confirm **Reset pairings** once more.

### Forget Ledger Nano X on your smartphone

1.  Open the Bluetooth settings of your smartphone.
2.  Select specific settings for your Ledger Nano X.
3.  Forget the device.

Now you can set up the pairing again by choosing your Ledger Nano X at any point in Ledger Live mobile that requires a device connection, for instance in the **Manager** tab.
