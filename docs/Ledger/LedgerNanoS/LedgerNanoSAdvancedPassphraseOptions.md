# Advanced Passphrase options

> The Ledger Nano S supports an ADVANCED security mode to manage different sets of accounts, each protected with a different passphrase. This feature is also referred to sometimes called "Plausible deniability".

These settings are useful to have 1 main account and 2 or several hidden accounts from the same wallet, with the same 24-word seed. But take care, these plausible deniability features are delicate to manage, as you are the only one to know a multitude of codes. if you ever lose them, Ledger nor anyone will be able to recover them for you. 

>Do not activate this option if you are not absolutely sure to understand it.

## What Is Plausible Deniability?

In Nano S, plausible deniability is a security feature to face the risk of being threatened and/or forced to give your PIN code. With this option, you will manage 2 PIN codes:

1.  **First PIN code** gives access to your main wallet, like a basic account with low amounts, to check daily payments.
2.  **Second PIN code**, linked to a specific passphrase you need to set up, opens an hidden account, for example to save large amounts, which will be used once in a while.

With this option, in case you are forced to recover a wallet from your 24-word backup, only the main wallet will be displayed, and the second account will remain hidden, as long as you don't reveal the attached passphrase. No one can know you have 2 PIN codes attached to your wallet, so you can reveal the first PIN code giving access to your daily wallet, to avoid having your savings stolen from your second wallet. As each PIN is using its own independent counter and PIN comparison is constantly done, it is highly unlikely for an unsuspecting sophisticated attacker to guess that a second PIN is enabled, providing that you give the first PIN to the attacker, and not possible to brute force one PIN knowing another one.

## Passphrase Attached To A Pin

>In your Nano S, go to SETTINGS > Security > Passphrase > Attach to a PIN

With this feature, you can create, open and manage a second (and hidden) wallet attached to a specific passphrase, wallet accessible when you connect your Nano S with another PIN code. As long as your session will be open with this PIN code, you will be able to access it. When you disconnect your Nano S or when you quit the standby mode, you will be asked a PIN code, then you can choose to reopen this one or enter the main PIN code.

1.  Open the "Settings" of the Nano S
2.  Select "Security"
3.  Select "Passphrase"
4.  Select "Attach to a PIN"
5.  Enter a second and new PIN code
6.  Confirm this new code
7.  Enter and confirm a secret passphrase (100 characters max)
8.  Enter your first main PIN code to validate

To access this hidden wallet, you have to disconnect the device and enter the second PIN. Otherwise, you will be in the "main" wallet.You can't set a third PIN code. If you ever set a new PIN code attached to a passphrase, it would erase the first one. To manage more than 1 hidden wallet you need to use the "temporary passphrase" option.

## How To Best Use The Passphrase Feature

Our recommendation is to use your current PIN for your day to day accounts, holding reasonable assets, and your alternate PIN for your savings account, holding higher value assets. This way, not only will your backup seed be protected by the passphrase, but your “duress” PIN will in fact be a real account with real transactions. This would be much more effective in a plausible deniability scenario.

## Temporary Passphrase

>In your Nano S, go to SETTINGS > Security > Passphrase > Set Temporary

With this feature, you can create, open or manage an hidden wallet, accessible only in this setting path. As long as your session will be open with this passphrase, you will be able to access it. When you disconnect your Nano S or when you quit the standby mode, this passphrase will be overwritten. You can create and manage as many temporary passphrases as you want, but only one by one - you can't open 2 or more temporary passphrases in the same session.

1.  Open the "Settings" of the Nano S
2.  Select "Security"
3.  Select "Passphrase"
4.  Select "Set temporary"
5.  Enter and confirm your secret passphrase (100 characters max)
6.  Enter your PIN code to validate

Then during the rest of your session until the Nano S is disconnected, you will run a new wallet attached to this passphrase. Next time you will enter your PIN code, you will open your main wallet, not this hiden account.

## **How To Recover Your Hidden Wallet(s) on a compatible device**

On your Nano S, just **[recover your 24 words]** and set your previous hidden passphrase as a temporary passphrase or as a hidden wallet attached to a PIN code.

### If you want to attach it to a passphrase:

1.  On your Nano S you must run the 24 words you previously ran when you set your passphrase. If you don't, reset your device and import the correct 24 words  
2.  Go to Settings > Security > Passphrase > Attach to a PIN  
3.  Choose a second PIN code and confirm it (you don't have to choose the same one as the previous one you set with the passphrase)  
4.  **Set the exact passphrase you want to recover** and confirm it  
5.  Validate by entering your first PIN code  
  
### If you want to set it as temporary:

1.  On your Nano S you must run the 24 words you previously ran when you set your passphrase. If you don't, reset your device and import the correct 24 words  
2.  Go to Settings > Security > Passphrase > Set temporary  
3.  **Set the exact passphrase you want to recover** and confirm it  
4.  Validate by entering your current PIN code

**HOW TO RECOVER YOUR HIDDEN WALLET(S) ON A COMPATIBLE WALLET**

If you ever lose your Ledger Nano S, you can restore your wallets and hidden wallets by importing your 24 words backup + your hidden passphrase, using any compatible wallet supporting BIP39 passphrases, on another Nano S, or on Trezor hardware wallet.  
You can also manually export your private keys using [an online tool for advanced users](https://www.ledgerwallet.com/support/bip39-standalone.html).
