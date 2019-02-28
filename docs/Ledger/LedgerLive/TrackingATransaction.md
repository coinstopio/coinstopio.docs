# Tracking A Transaction

Once a transaction has been sent, it is broadcasted to the network for validation. Track its status in the Ledger Live application to know when it is confirmed and when your balance gets updated.

**BLOCKCHAIN VALIDATION**

-   Transactions are validated by the amount of blocks that include the transaction: block confirmations. At a certain amount of block confirmations, a transaction is considered as confirmed
-   The minimum number of confirmations varies between cryptocurrencies, as each blockchain has its own block time. By default, Ledger Live sets the minimum number of confirmations to the amount of blocks that fit in 30 minutes
-   You can configure the required number of confirmations in **settings > currencies**. For crypto assets that function like Bitcoin, a high number of confirmations makes a transaction irreversible

**TRANSACTION STATES**

The operations list in your portfolio indicates the transaction state based on the number of confirmations.

**PENDING**

-   A transaction is pending if it hasn't received any confirmations yet
-   Transactions that included higher network fees normally don't stay pending for a long time
-   If a transaction included lower network fees, it can remain pending for a longer time
-   Learn [how to increase the fees on a transaction](https://coinstop.kayako.com/article/176-transaction-remains-unconfirmed) to increased the likelihood the transaction is picked up by the miners (currently only available on the Ledger Chrome extension, feature to be added to Ledger Live in the future)

**CONFIRMING**

-   Once a transaction has had its first block confirmation, its status switches to **confirming**. This status remains  until the required number of confirmations is reached
-   Click a transaction in the **last operations** list to open the **operations details** to track its status
-   Click **view in explorer** to look up the transaction in a third-party blockchain network explorer

**CONFIRMED**

-   After reaching the required number of confirmations, the transaction status switches to **confirmed**
-   All confirmed transactions combined make up the balance of your accounts and portfolio
-   Cryptocurrency in your portfolio can only be sent if the transaction, with which you received them, is confirmed