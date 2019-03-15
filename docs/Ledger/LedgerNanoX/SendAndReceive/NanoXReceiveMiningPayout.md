
# Receive mining proceeds

Participants in mining activities may want to securely store their mining proceeds by using a Ledger device. This article explains why sending a large amount of small transactions to a hardware wallet is troublesome, offers potential solutions and provides instructions on how to properly send mining proceeds to an address controlled by your Ledger device.

Failing to follow these instructions may lead to your funds becoming inaccessible on a Ledger device.

## Receiving many small transactions is troublesome

Receiving a large number of small payments, or _dust payments_, on an address controlled by your hardware wallet causes:

-   the saturation of the synchronization of your Blockchain transactions; and
-   an extremely long duration of transaction construction or validation.

Therefore, hardware wallets are not directly suited for receiving a large amount of small transactions, such as the proceeds of mining activities.

Imagine that you have received 1,000 payments of 0.001 BTC and that you want to spend the total of 1 BTC. The secure chip in the hardware wallet will then have to construct a transaction of 1,000 inputs and sign each single input. This might take a few hours or might not succeed at all, since the chip may overheat or make a computation error.

## If you've received a lot of small payments

If you have already sent a large number of small payments to your hardware wallet:

-   Try to consolidate your coins by sending a few larger payments to yourself. For example, if you have received 1,000 times 0.001 BTC, consolidate these inputs by sending 0.1 BTC to yourself and repeat this 10 times.
-   Alternatively, import your 24-word recovery phrase into a software wallet, preferably an offline one, and empty your wallet into an address that is derived from a newly generated seed.

## Batch transactions to prevent problems

-   Set up a software wallet that receives the small payments;
-   Regularly batch these proceeds into a larger transaction to send onto a hardware wallet.