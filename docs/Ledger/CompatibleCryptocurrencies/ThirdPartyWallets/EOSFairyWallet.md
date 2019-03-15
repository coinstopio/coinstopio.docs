# (DRAFT) Fairy-Wallet (EOS)

https://support.ledgerwallet.com/hc/en-us/articles/360008913653

Install the EOS app on your Ledger Nano S to manage EOS with the [Fairy-wallet](https://github.com/tarassh/fairy-wallet/releases/). The EOS app is developed and supported by the [EOS community](https://eos.io/).

## Before you start

-   You've [initialized](https://support.ledgerwallet.com/hc/en-us/articles/360000613793) your Ledger Nano S.
-   The latest firmware is [installed](https://support.ledgerwallet.com/hc/en-us/articles/360002731113).
-   Ledger Live is [ready to use](https://support.ledgerwallet.com/hc/en-us/articles/360006395233).

## Install the EOS app

1.  Open the **Manager** in Ledger Live.
2.  Connect and unlock your Ledger Nano S.
3.  If asked, allow the manager on your device by pressing the right button.
4.  Find **EOS** in the app catalog.
5.  Click the **Install** button of the app.
    -   An installation window appears.
    -   Your device will display **Processing...**
    -   The app installation is confirmed.

## Next steps

-   Check the  [user guide](https://github.com/tarassh/fairy-wallet/wiki)  for step by step instructions.
-   Join the Fairy-wallet  [Telegram](https://t.me/fairywallet) or open an issue on  [Github](https://github.com/tarassh/fairy-wallet/issues)  if you require assistance.

EOS accounts can not be added to Ledger Live.

  

  

https://github.com/tarassh/fairy-wallet/wiki

Verify you have:

-   An [initialized](https://support.ledgerwallet.com/hc/en-us/articles/360000613793) Ledger Nano S,
-   The latest firmware [installed](https://support.ledgerwallet.com/hc/en-us/articles/360002731113),
-   Windows 10, macOS 10.8+ or Linux,
-   Installed the [Ledger Live](https://www.ledgerwallet.com/live) app.

Welcome to the Fairy wallet wiki, Ledger Nano S compatible wallet for EOS software.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/application/Wallet.png)

  

To download the latest release version of the application use one the following links:

-   for [MacOS](https://github.com/tarassh/fairy-wallet/releases/download/v0.9.6/FairyWallet-0.9.6.dmg)
-   for [Windows](https://github.com/tarassh/fairy-wallet/releases/download/v0.9.6/FairyWallet.Setup.0.9.6.exe)
-   for [Linux](https://github.com/tarassh/fairy-wallet/releases/download/v0.9.6/fairy-wallet_0.9.6_amd64.deb)

Release notes: [https://github.com/tarassh/fairy-wallet/releases](https://github.com/tarassh/fairy-wallet/releases)

NOTE: application on Linux may require additional permissions for the device. To add permissions, use this [script](https://github.com/LedgerHQ/udev-rules/blob/master/add_udev_rules.sh). Windows users may experience slow response from the device due to driver issues.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/new-connect.png)

To connect to EOS Mainnet you can use one of the following endpoints:

-   [http://api.cypherglass.com](http://api.cypherglass.com/) - operated by [Cypherglass](https://www.cypherglass.com/)
-   [https://eos.greymass.com](https://eos.greymass.com/) - operated by [Greymass](https://greymass.com/)
-   [https://api.eossweden.se](https://api.eossweden.se/) - operated by [Sw/eden](https://eossweden.org/)
-   [https://nodes.eos42.io](https://nodes.eos42.io/) - operated by [EOS42](https://www.eos42.io/)
-   [http://api-mainnet.starteos.io](http://api-mainnet.starteos.io/) - operated by [Starteos](https://www.starteos.io/)
-   [https://eosbp.atticlab.net](https://eosbp.atticlab.net/) - opeated by [AtticLab](https://atticlab.net/)
-   [https://api1.eosdublin.io](https://api1.eosdublin.io/) - operated by [eosDublin](https://www.eosdublin.com/)
-   [https://node1.eosphere.io](https://node1.eosphere.io/) - operated by [EOSphere](https://www.eosphere.io/)
-   [https://node2.eosphere.io](https://node2.eosphere.io/) - operated by [EOSphere](https://www.eosphere.io/)

EOS, unlike other cryptocurrencies, requires personal accounts. Accordingly, to perform any actions, you need to have one. To create an account, you need to retrieve Public Key from the Ledger device. To do that, follow this steps:

1.  Connect and unlock your device with your PIN code.
2.  Open the Fairy Wallet app.
3.  Connect to EOS network entering one of the listed [endpoints](https://github.com/tarassh/fairy-wallet#connect-to-mainnet).

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/create-account-connect.png)

1.  **Create account** window will appear. To create an account, retrieve a public key from the device by clicking on the **key icon**.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/public-key-get.png)

1.  The “**Get Public Key**” window will appear. Press **Verify** to start a public key verification process.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/public-key-verify.png)

1.  Match the key displayed on the device with the key displayed on the screen and press a right button on the device to confirm.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/create-account-pk-ledger.png)

1.  Press **COPY TO CLIPBOARD** button to go next.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/public-key-verify-hw.png)

1.  This screen provides a **Create Account** functionality directly from [https://create-eos-account-for.me](https://create-eos-account-for.me/) service developed by [Lecko(Taewoong La)](https://github.com/DiyLecko).

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/choose-account-name.png)

Go through the payment process and create your personal account. Make sure that the Owner's Public Key and the Active Public Key match the Public key retrieved from a Ledger device. Choose a payment method and proceed to payment. When an account is created press **LOGIN** at the bottom of the screen.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/success.png)

NOTE: This solution is optional, You can use any other existing services to create an account. The primary requirement is to use public key retrieved from the device. Here is the list of other available services:

-   [https://eostoolkit.io/account/create](https://eostoolkit.io/account/create)
-   [https://www.zeos.co](https://www.zeos.co/)
-   [https://eos-account-creator.com](https://eos-account-creator.com/)

1.  Click on the account name to enter.

![](https://github.com/tarassh/fairy-wallet/raw/master/resources/wiki/createaccount/account-select.png)