# Hide accounts with a passphrase

> Warning: this tutorial is for advanced users.

_Firmware compatibility:_

- _1.3.1 (+):_ [_These options are available directly under the Settings menu on the Ledger Nano S._](https://support.ledgerwallet.com/hc/en-us/articles/115005214529-Advanced-Passphrase-options)

- _1.0 to 1.2: Update your Ledger Nano S or contact us for advanced developer tools._

## **What is a hidden passphrase?**

The hidden passphrase is a 25th word on top of your 24 word recovery phrase, but one that you need to remember and never write down. It generates a new identity: there is no right or wrong passphrase.

## **The hidden passphrase is used for two reasons**

1. Protection of your 24 words recovery phrase if your accounts are behind a passphrase then you are protected.

2. "Plausible deniability" is a security feature that combats the risk of being threatened and/or forced to enter your PIN code. With this option, you can manage two PIN codes, unlocking two separate accounts:

- Your **first PIN code** provides access to your main wallet, like a basic account, with low amounts used for daily payments and small transactions.

- **Second PIN code**, linked to a specific passphrase you need to set up, opens an hidden account, to save large amounts, which will only be used occasionally. With this option, in case you are forced to recover a wallet from your 24-word backup, only the main wallet will be displayed, and the second account will remain hidden, as long as you don't reveal the attached passphrase.

Note that all applications on your Ledger device (Bitcoin, Ethereum, FIDO…) are affected by the passphrase identity change.

  
## **How to create a hidden passphrase and its PIN code**

On your Ledger Nano S:

"Settings" > "Security" >  "Passphrase" >  "Attach to a PIN"

1. Enter a second and new PIN code

2. Confirm this new code

3. Enter and confirm a secret passphrase (100 characters max)

4. Enter your first main PIN code to validate

To access this hidden wallet, you have to disconnect the device and enter the second PIN. Otherwise, you will be in the "main" wallet.  
You can't set a third PIN code. If you ever set a new PIN code attached to a passphrase, it would erase the first one and the assets held by it.

How to best use the passphrase feature: our recommendation is to use your current PIN for your day to day accounts, and your alternate PIN for your savings account, holding a larger amount of assets. This way, not only will your backup seed be protected by the passphrase, but your “duress” PIN code will in fact be a real account with real transactions. This would be much more effective for a plausible deniability scenario.

## **Temporary Passphrase**

With this feature, you can create, open or manage an hidden wallet, accessible only in this setting path. As long as your session will be open with this passphrase, you will be able to access it. When you disconnect your Nano S or when you quit the standby mode, this passphrase will be overwritten.

You can create and manage as many temporary passphrases as you want, but only one by one - you can't open two or more temporary passphrases in the same session:

"Settings" > "Security" > "Passphrase" > "Set temporary"

1. Enter and confirm your secret passphrase (100 characters max)

2. Enter your PIN code to validate

Then during the rest of your session until the Nano S is disconnected, you will run a new wallet attached to this passphrase. Next time you will enter your PIN code, you will open your main wallet, not this hidden account.

## **How to recover your hidden wallet(s) on a Ledger Nano S**

On your Ledger Nano S you need to [recover your 24 words](https://support.ledgerwallet.com/hc/en-us/articles/115005165309-How-to-import-recover-a-backup-on-a-Nano-S-) and set your previous hidden passphrase as a temporary passphrase or as a hidden wallet attached to a PIN code.

### If you want to attach it to a passphrase:

1. on your Nano S you must run the 24 words you previously ran when you set your passphrase. If you don't, reset your device and import the correct 24 words

2. go to "Settings" > "Security" > "Passphrase" > "Attach to a PIN"

3. choose a second PIN code and confirm it (you don't have to choose the same one as the previous one you set with the passphrase)

4. set the exact passphrase you want to recover and confirm it

5. validate by entering your first PIN code

### If you want to set it as temporary passphrase:

1. on your Nano S you must run the 24 words you previously ran when you set your passphrase. If you don't, reset your device and import the correct 24 words

2. go to "Settings" > "Security" > "Passphrase" > "Set temporary"

3. set the exact passphrase you want to recover and confirm it

4. validate the passphrase by entering your current PIN code

## **How to recover your hidden wallet(s) on a compatible wallets**

If you ever lose your Ledger Nano S, you can restore your main wallets and hidden wallets by importing your 24 words backup and your hidden passphrase, using any compatible wallet that supports BIP39 passphrases, or on another Ledger Nano S hardware wallet.

You can also manually export your private keys using  [an online tool for advanced users](https://www.ledgerwallet.com/support/bip39-standalone.html).