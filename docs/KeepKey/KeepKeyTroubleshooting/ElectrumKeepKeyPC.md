# (DRAFT) Electrum KeepKey Integration for Windows (7, 8 & 10)

To setup KeepKey integration with Electrum, here are the following steps:  
  
I. Download and Install Python v2.7.x (Latest Version): HTTPS://WWW.PYTHON.ORG/DOWNLOADS/WINDOWS/  
  
Make sure you note which type, 32-bit or 64-bit, you install as you will need this information in a later step.  
  
II. Install Microsoft Visual C++ Compiler for Python 2.7: HTTP://WWW.MICROSOFT.COM/EN-US/DOWNLOAD/DETAILS.ASPX?ID=44266

III. Install KeepKey Python Client.  
Open Command Prompt (cmd)  
Enter following command - C:\python27\scripts\pip.exe install keepkey

IV. Download and Install PyQt4 for Python v2.7: HTTPS://WWW.RIVERBANKCOMPUTING.COM/SOFTWARE/PYQT/DOWNLOAD  
Download and install, matching the same 32-bit or 64-bit type you chose for Python in the first step.  
  
V. Download and Unzip Electrum: https://download.electrum.org/2.6.4/Electrum-2.6.4.zip  
Recommendation is to unzip to C:\ creating the folder C:\Electrum-2.6.4

VI. Launch Electrum.  
Open Command Prompt (cmd)  
Enter following command - cd C:\Electrum-2.6.4 (Or wherever you have unzipped the Electrum-2.6.4 directory)  
Enter following command - C:\Python27\python.exe electrum