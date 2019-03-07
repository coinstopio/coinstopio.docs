# Obtaining xPub On Windows

To obtain xPub on **Windows**, please follow the steps detailed below:

1.  [Download](https://www.python.org/downloads/) and Install Python v2.7.x (Latest Version)
2.  Install Cython  
      
    _Open Command Prompt (cmd) and enter the below command:_  
      
    _C:\python27\scripts\pip.exe install cython_
3.  [Download and install Microsoft Visual  C++  Compiler for Python 2.7](http://WWW.MICROSOFT.COM/EN-US/DOWNLOAD/DETAILS.ASPX?ID=44266)
4.  Install KeepKey Python Client  
      
    _Open Command Prompt (cmd) and enter below command:  
      
    C:\python27\scripts\pip.exe install HTTPS://GITHUB.COM/KEEPKEY/PYTHON-KEEPKEY/ARCHIVE/MASTER.ZIP  
    Download Chrome-Proxy-Master_
5.  Download and Extract Chrome-Proxy-Master  
      
    _Click Download Zip  
    Extract and save to C:\  
    Retrieve xPub key_
6.  How to retrieve the xPub key  
      
    _Open Command Prompt (cmd) and enter the below command:  
      
    cd c:\python27_
7.  Witt CMD still open, enter the below command:  
    _python.exe Scripts\keepkeyctl get_public_node -n "44'/0'/0'"_  
      
    Enter PIN according to KeepKey screen and placement of numbers in command prompt