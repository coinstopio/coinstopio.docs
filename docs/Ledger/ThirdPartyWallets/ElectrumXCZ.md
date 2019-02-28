# (DRAFT) Electrum (XZC)

https://support.ledgerwallet.com/hc/en-us/articles/360006543693

Install the Zcoin app on your Ledger Nano S or Ledger Blue device to manage XZC with the [Electrum-XZC](https://github.com/zcoinofficial/electrum-xzc/releases/latest) application. The app is developed and supported by the [Zcoin community](https://zcoin.io/).

## Before you start

-   Ledger Live is [ready to use](https://support.ledgerwallet.com/hc/en-us/articles/360006395233).
-   The latest firmware is [installed](https://support.ledgerwallet.com/hc/en-us/articles/360002731113) on your Ledger device.
-   The Bitcoin app is installed, since Zcoin requires it.

## Install the Zcoin app

1.  Open the **Manager** in Ledger Live.
2.  Connect and unlock your device.
3.  If asked, allow the manager on your device.
4.  Find **Zcoin** in the app catalog.
5.  Click the **Install** button of the app.
    -   An installation window appears.
    -   Your device will display **Processing...**
    -   The app installation is confirmed.

## Next steps

-   Check the [Zcoin user guide](https://zcoin.io/using-zcoin-with-ledger-on-electrum/) for step by step instructions.
-   Reach out to the [Zcoin community on Reddit](https://www.reddit.com/r/zcoin/) if you require assistance.

Zcoin accounts can not be added to Ledger Live.

  

  

https://zcoin.io/using-zcoin-with-ledger-on-electrum/

## Download and Installation

First [download](https://github.com/zcoinofficial/electrum-xzc/releases/latest) the latest Electrum-XZC binaries for your operating system and install these on your computer.

## Set up Electrum-XZC

In the screen **How do you want to connect to a server?**, please select _Auto connect_.  
In the next screen, pick a name for a new wallet or keep the default name _default_wallet_.  
Then choose _Standard wallet_.

![](https://i.imgur.com/Jrfd3va.png)

In the **Keystore** dialogue, pick _Use a hardware device_.

![](https://i.imgur.com/WQtlNG0.png)

Now pick your Ledger.

![](https://i.imgur.com/1PyH6OH.png)

The derivation path listed in the **Derivation** dialogue should be accepted as suggested. Advanced users can tweak this according to their needs.

![](https://i.imgur.com/A0iLpNU.png)

After you have clicked _Next_, Electrum-XZC will synchronise your account. This might take a while.

## Sending Zcoin

Before you can sign transactions with your Ledger, you first have to install the Zcoin app in Ledger Manager and then start it on your Ledger. If you then want to send XZC, you have to sign it by validating it on your Ledger.

![](https://i.imgur.com/tdQIo0X.png)

### Note to Ubuntu Users

The following additional steps need to taken for Electrum-XZC to work:

```
- apt-get install libusb-1.0-0-dev
- apt-get install libudev-dev
- ln -s /lib/x86_64-linux-gnu/libudev.so.1 /lib/x86_64-linux-gnu/libudev.so
- pip install btchip-python
```