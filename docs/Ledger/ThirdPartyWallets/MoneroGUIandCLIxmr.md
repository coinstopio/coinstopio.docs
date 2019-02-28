# (DRAFT) Monero GUI & CLI (XMR)

https://support.ledgerwallet.com/hc/en-us/articles/360006352934

# Monero (XMR) - Advanced

Monero (XMR) can be managed from the Ledger Nano S device with the Monero Graphical User Interface (GUI) after you've created an account with the Monero Command Line Interface (CLI).

#### Need assistance?

Please refer to the **[Monero Reddit community](https://www.reddit.com/r/Monero/)** for more information and troubleshooting

## Before you start

-   Make sure your Ledger Nano S runs the latest firmware and [has been initialized](https://support.ledgerwallet.com/hc/en-us/articles/360000613793)
-   Download the latest versions of both the [GUI and CLI Monero client](https://getmonero.org/downloads/)
-   Close all Monero related processes

## Step by step instructions

### Install Monero app on your Ledger device

1.  Open the **Manager** in Ledger Live.
2.  Connect and unlock your Ledger device.
3.  If asked, allow the manager on your device by pressing the right button.
4.  Find **Monero** in the app catalog.
5.  Click the **Install** button of the app.
    1.  An installation window appears.
    2.  Your device will display **Processing...**
    3.  The app installation is confirmed.

### Select your operating system

Windows

**Step 1** - Go to the directory / folder `monero-wallet-gui.exe` (GUI v0.12.1.0) is located (note that `monero-wallet-cli.exe` will be in the same directory / folder as `monero-wallet-gui.exe`).

**Step 2** - Open a new command prompt / powershell. This is done by first making sure your cursor isn't located on any of the files and subsequently doing SHIFT + right click. It will give you an option to "Open command window here". If you're using Windows 10, it'll, most likely, give you an option to open the Powershell.

**Step 3** - Now type:  
`monero-wallet-cli.exe --generate-from-device <new-wallet-name> --restore-height 1580000 --subaddress-lookahead 3:200` **(Win 7 + 8)**  
`.\monero-wallet-cli.exe --generate-from-device <new-wallet-name> --restore-height 1580000 --subaddress-lookahead 3:200` **(Win 10)**  
Note that <new-wallet-name> is simply a placeholder for the actual wallet name. If you, for instance, want to name your wallet `MoneroWallet`, the command would be as follows:  
`monero-wallet-cli.exe --generate-from-device MoneroWallet --restore-height 1580000 --subaddress-lookahead 3:200` **(Win 7 + 8)**  
`.\monero-wallet-cli.exe --generate-from-device MoneroWallet --restore-height 1580000 --subaddress-lookahead 3:200` **(Win 10)**

**Step 4** - The CLI will, after executing aforementioned command, prompt your for a password. Make sure to set a strong password and confirm it thereafter.

**Step 5** - The Ledger will ask whether you want to export the private view key or not. First and foremost, your funds cannot be compromised with merely the private view key. Exporting the private view key enables the client (on the computer - Monero v0.12.1.0) to scan blocks looking for transactions that belong to your wallet / address. If this option is not utilized, the device (Ledger) will scan blocks, which will be significantly slower. There is, however, one caveat. That is, if your system gets compromised, the adversary will potentially be able to compromise your private view key as well, which is detrimental to privacy. This is virtually impossible when the private view key is not exported.

**Step 6** - You may have to hit confirm twice before it proceeds.

**Step 7** - Your Ledger Monero wallet will now be generated. Note that this may take up to 5-10 minutes. Furthermore, there will be no immediate feedback in the CLI nor on the Ledger.

**Step 8** - You may, after the CLI has generated your wallet, get an error about the wallet not being connected to the daemon. You can ignore that for now.

**Step 9** - Type `exit` into `monero-wallet-cli.exe` to close the CLI.

**Step 10** - Note that your wallet files will be stored in the same directory / folder as `monero-wallet-gui.exe` & `monero-wallet-cli.exe`. This may be a bit inconvenient. Fortunately, you can simply copy the wallet files to a different preferred directory / folder.

**Step 11** - Open GUI v0.12.1.0. If you have already created a wallet in the GUI, click `Cancel` when it prompts you for the password of your current wallet. This should bring you back to the wizard. If you haven't already created a wallet, you should automatically start in the wizard.

**Step 12** - The first page of the wizard is language selection, which looks like [this](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md#1-choose-a-language) . Select your desired language to proceed.

**Step 13** - On the second page of the wizard, which looks like [this](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md#2-create-a-wallet), select `Open a wallet from file`.

**Step 14** - Select the wallet file (which, to reiterate, is stored in the same directory / folder as `monero-wallet-gui.exe`) you just created with the CLI.

**Step15** - Congratulations, you can now use your Ledger Monero wallet with the GUI! If you have any further questions with the GUI, please refer to [this guide](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md).

Linux

**Step 1** - Go to the directory / folder `monero-wallet-gui` (GUI v0.12.1.0) is located (note that `monero-wallet-cli` will be in the same directory / folder as `monero-wallet-gui`).

**Step 2** - Open a new terminal.

**Step 3** - Now type:  
`./monero-wallet-cli --generate-from-device <new-wallet-name> --restore-height 1580000 --subaddress-lookahead 3:200`  
Note that <new-wallet-name> is simply a placeholder for the actual wallet name. If you, for instance, want to name your wallet `MoneroWallet`, the command would be as follows:  
`./monero-wallet-cli --generate-from-device MoneroWallet --restore-height 1580000 --subaddress-lookahead 3:200`

**Step 4** - The CLI will, after executing aforementioned command, prompt your for a password. Make sure to set a strong password and confirm it thereafter.

**Step 5** - The Ledger will ask whether you want to export the private view key or not. First and foremost, your funds cannot be compromised with merely the private view key. Exporting the private view key enables the client (on the computer - Monero v0.12.1.0) to scan blocks looking for transactions that belong to your wallet / address. If this option is not utilized, the device (Ledger) will scan blocks, which will be significantly slower. There is, however, one caveat. That is, if your system gets compromised, the adversary will potentially be able to compromise your private view key as well, which is detrimental to privacy. This is virtually impossible when the private view key is not exported.

**Step 6** - You may have to hit confirm twice before it proceeds.

**Step 7** - Your Ledger Monero wallet will now be generated. Note that this may take up to 5-10 minutes. Furthermore, there will be no immediate feedback in the CLI nor on the Ledger.

**Step 8** - You may, after the CLI has generated your wallet, get an error about the wallet not being connected to the daemon. You can ignore that for now.

**Step 9** - Type `exit` into `monero-wallet-cli` to close the CLI.

**Step 10** - Note that your wallet files will be stored in the same directory / folder as `monero-wallet-gui` & `monero-wallet-cli`. This may be a bit inconvenient. Fortunately, however, you can simply copy the wallet files to a different preferred directory / folder.

**Step 11** - Open GUI v0.12.1.0. If you have already created a wallet in the GUI, click `Cancel` when it prompts you for the password of your current wallet. This should bring you back to the wizard. If you haven't already created a wallet, you should automatically start in the wizard.

**Step 12** - The first page of the wizard is language selection, which looks like [this](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md#1-choose-a-language).

**Step 13** - On the second page of the wizard, which looks like [this](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md#2-create-a-wallet), select `Open a wallet from file`.

**Step 14** - Select the wallet file (which, to reiterate, is stored in the same directory / folder as `monero-wallet-gui`) you just created with the CLI.

Congratulations, you can now use your Ledger Monero wallet with the GUI! If you have any further questions with the GUI, please refer to [this guide](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md).

Mac

**Step 1** - Use Finder to browse to the directory / folder `monero-wallet-gui.app` (GUI v0.12.1.0) is located.

**Step 2** - Right click on `monero-wallet-gui.app` -> `Show contents`

**Step 3** - You should now see `monero-wallet-cli`

**Step 4** - Go to your desktop.

**Step 5** - Open a new terminal.

**Step 6** - Drag `monero-wallet-cli` in the terminal. It should add the full path to the terminal. Do not hit enter.

**Step 7** - Now type:  
`--generate-from-device <new-wallet-name> --restore-height 1580000 --subaddress-lookahead 3:200`  
Note that <new-wallet-name> is simply a placeholder for the actual wallet name. If you, for instance, want to name your wallet `MoneroWallet`, the command would be as follows:  
`--generate-from-device MoneroWallet --restore-height 1580000 --subaddress-lookahead 3:200`  
Note that aforementioned text will be appended to the path of `monero-wallet-cli`. Thus, before you hit enter, your terminal should look like:  
`/full/path/to/monero-wallet-cli --generate-from-device <new-wallet-name> --restore-height 1580000 --subaddress-lookahead 3:200`  
Where the full path is, intuitively, the actual path on your Mac OS X.

**Step 8** - The CLI will, after executing aforementioned command, prompt your for a password. Make sure to set a strong password and confirm it thereafter.

**Step 9** - The Ledger will ask whether you want to export the private view key or not. First and foremost, your funds cannot be compromised with merely the private view key. Exporting the private view key enables the client (on the computer - Monero v0.12.1.0) to scan blocks looking for transactions that belong to your wallet / address. If this option is not utilized, the device (Ledger) will scan blocks, which will be significantly slower. There is, however, one caveat. That is, if your system gets compromised, the adversary will potentially be able to compromise your private view key as well, which is detrimental to privacy. This is virtually impossible when the private view key is not exported.

**Step 10** - You may have to hit confirm twice before it proceeds.

**Step 11** - Your Ledger Monero wallet will now be generated. Note that this may take up to 5-10 minutes. Furthermore, there will be no immediate feedback in the CLI nor on the Ledger.

**Step 12** - You may, after the CLI has generated your wallet, get an error about the wallet not being connected to the daemon. You can ignore that for now.

**Step 13** - Type `exit` into `monero-wallet-cli` to close the CLI.

**Step 14** - Note that your wallet files will, most likely, be stored in `~`, which is short for `/Users/<username>` on Mac OS X. This may be a bit inconvenient. Fortunately, however, you can simply copy the wallet files to a different preferred directory / folder.

**Step 15** - Open GUI v0.12.1.0. If you have already created a wallet in the GUI, click `Cancel` when it prompts you for the password of your current wallet. This should bring you back to the wizard. If you haven't already created a wallet, you should automatically start in the wizard.

**Step 16** - The first page of the wizard is language selection, which looks like [this](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md#1-choose-a-language).

**Step 17** - On the second page of the wizard, which looks like [this](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md#2-create-a-wallet). Select `Open a wallet from file`.

**Step 18** - Select the wallet file (the .keys file, which, to reiterate, is stored in either `Users/<username>` or in your preferred directory / folder) you just created with the CLI.

# Start sending and receiving Monero

Congratulations, you can now use your Ledger Monero wallet with the GUI! If you have any further questions with the GUI, please refer to [this guide](https://github.com/monero-ecosystem/monero-GUI-guide/blob/master/monero-GUI-guide.md).