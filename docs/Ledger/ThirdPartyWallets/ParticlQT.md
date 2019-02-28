# (DRAFT) Particl-Qt (PART)

https://support.ledgerwallet.com/hc/en-us/articles/360007687153

Install the Particl app on your Ledger Nano S to manage PART tokens with the Particl-Qt wallet. The Particl app is developed and supported by the [Particl community](https://particl.io/).

## Before you start

-   You've [initialized](https://support.ledgerwallet.com/hc/en-us/articles/360000613793) your Ledger Nano S.
-   The latest firmware is [installed](https://support.ledgerwallet.com/hc/en-us/articles/360002731113).
-   Ledger Live is [ready to use](https://support.ledgerwallet.com/hc/en-us/articles/360006395233).

## Install the Particl app

1.  Open the **Manager** in Ledger Live.
2.  Connect and unlock your Ledger Nano S.
3.  If asked, allow the manager on your device by pressing the right button.
4.  Find **Particl** in the app catalog.
5.  Click the **Install** button of the app.
    -   An installation window appears.
    -   Your device will display **Processing...**
    -   The app installation is confirmed.

## Next steps

-   Check the [Particl user guide](https://particl.wiki/ledger) for step by step instructions.
-   Reach out to the [Particl community](https://particl.io/) for support.

Particl accounts can not be added to Ledger Live.

  

  

https://particl.wiki/ledger

## What is the Ledger Nano S?

  

[![ledger-wallet.jpg](https://particl.wiki/_media/ledger-wallet.jpg?w=350&tok=52adbb "ledger-wallet.jpg")](https://particl.wiki/_media/ledger-wallet.jpg "ledger-wallet.jpg")The [Ledger Nano S](https://www.ledger.com/) is a hardware wallet, a special type of bitcoin wallet which stores the user's private keys in a secure hardware device. They have major advantages over standard software wallets: private keys are stored in a secure chip, and cannot be transferred out of the device in plaintext. That means your funds are safe even when connected to an infected or malicious computer or a phishing/scam web page. For these reasons, we highly recommend users to protect their funds by setting up a Ledger Nano S.

  

## Requirements

  

Before starting the setup process, make sure you have:

-   **Ledger Nano S** hardware wallet – initialized and [updated to latest firmware](https://support.ledgerwallet.com/hc/en-us/articles/360002731113-Update-Ledger-Nano-S-firmware)
    
-   **Ledger Live** app [ready to use](https://support.ledgerwallet.com/hc/en-us/articles/360006395233)
    
-   **[Particl-Qt](https://github.com/particl/particl-core/releases)** wallet installed and fully synced to the Particl network
    

  

### Linux users

  

Make sure you have added the `udev` rules to allow device access – see [Fix connection issues](https://support.ledgerwallet.com/hc/en-us/articles/115005165269-Fix-connection-issues) (under Linux tab) for more info.

If you already have a working Ledger wallet, you can skip this.

  

## Install the Particl app on your device

  

  

**For more information**, see **[Particl on Ledger](https://support.ledgerwallet.com/hc/en-us/articles/360007687153)** guide on Ledger Support

  

1.  Open the **Manager** in Ledger Live.
    
2.  Connect and unlock your Ledger Nano S.
    
3.  If asked, allow the manager on your device by pressing the right button.
    
4.  Find **Particl** in the app catalog.
    
5.  Click the **Install** button of the app.
    
    5.1 An installation window appears.
    
    5.2 Your device will display **Processing…**
    
    5.3 The app installation is confirmed.
    
      
    

  

## Set up a new Ledger account on Particl-Qt

  

  

  

[![](https://particl.wiki/_media/images/01_startup.png?w=500&tok=49f795)](https://particl.wiki/_media/images/01_startup.png)

  

  

[![](https://particl.wiki/_media/images/02_startup.png?w=500&tok=ee04da)](https://particl.wiki/_media/images/02_startup.png)

  

  

  

**If you already have a wallet on this computer,** make sure to back the **[wallet.dat](https://particl.wiki/particl-clients#file_structure "particl-clients")** file up by renaming or moving it elsewhere!

  

1.  Launch Particl-Qt on your computer
    
2.  Go to **File → HD Wallet** (if it's the first time you're setting up a wallet on this computer or if you don't have any `wallet.dat` file in your [Particl config folder](https://particl.wiki/particl-clients#file_structure "particl-clients"), then Particl-Qt will automatically bring you to this section)
    
3.  Click on the **Hardware Device** tab
    
4.  Connect your Ledger Nano S to your computer via USB
    
5.  Make sure the device is properly unlocked and connected to Ledger Live
    
6.  Click on **Import**
    
7.  When your Particl-Qt wallet says _Waiting for device_, follow the instructions displayed on your Ledger hardware wallet screen
    
8.  Your Particl-Qt client is now ready to be used in conjunction with your Ledger hardware wallet
    

  

## Send Particl using your Ledger wallet

  

  

  

[![](https://particl.wiki/_media/images/03_send.png?w=350&tok=1deac7)](https://particl.wiki/_media/images/03_send.png)

  

  

[![](https://particl.wiki/_media/images/04_send.png?w=350&tok=4f509b)](https://particl.wiki/_media/images/04_send.png)

  

  

[![](https://particl.wiki/_media/images/05_send.png?w=350&tok=2bcad7)](https://particl.wiki/_media/images/05_send.png)

  

  

1.  Open your Particl-Qt client containing your Ledger hardware wallet (as set up in the steps above)
    
2.  Connect your Ledger hardware wallet to your computer and unlock it using your PIN code
    
3.  Select and start the Particl application on your Ledger hardware wallet
    
4.  Click on Particl-Qt's **Send** tab
    
5.  Enter your transaction details (PART amount and destination address)
    
6.  Click **Send → Yes**
    
7.  Particl-Qt will prompt you to follow the steps displayed on your Ledger hardware wallet's screen
    
8.  Confirm the transaction on your device if the transaction details are correct
    

  

**To enable cold staking** on your Ledger Nano S, follow the steps in this [hardware cold staking tutorial](https://particl.wiki/ledger_staking "ledger_staking").