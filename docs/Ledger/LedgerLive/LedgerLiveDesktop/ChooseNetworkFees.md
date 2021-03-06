
<needs link>

# Choose Network Fees

## The Use Of Network Fees

-   The security of a blockchain network like Bitcoin generally depends on the amount of work done by miners. Miners are the computers competing to solve an algorithm that allows them to receive the block reward, the fees, and the ability to propagate the next block in the chain.
-   The miner that proposes the next block of transactions to the network must also provide proof of the work done required to create the block.
-   If the transactions are valid and the proof of work is sufficient, the miner may collect the fees offered in the included transactions, as a reward for the work done.

## Choose Your Network Fees

When **[sending cryptocurrency]**, the network fees you choose determine your priority in the queue of pending transactions, the mempool. Miners are incentivised to prioritise transactions that offer high fees.

Ledger Live offers a three (3) tiered fee structure, as well as a custom fee option:

-   **High:** the transaction _should_ be included in the next block (~10 min for Bitcoin)
-   **Standard:** the transaction _should_ be included within 3 blocks (~30 min for Bitcoin)
-   **Low:** the transaction _should_ be included within 6 blocks (~60 min for Bitcoin)

>Choose high fees if you need a faster confirmation, or a lower fee if you can wait a little longer.

## Calculation Of Fees

The fee amount is calculated dynamically and will be dependent on the transaction file size. Therefore, a transaction with a more inputs or outputs will be more expensive than one with fewer inputs and outputs.
