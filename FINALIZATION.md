When someone submits a transaction if follows a lifecycle.

- The transaction is gossiped across the blockchain to a block proposer.
- The block proposer receives and includes in a block.
- The block is broadcasted.

These conditions lead to forks off the blockchain, and they need to figure it out which one is canonical.

When a transaction is expunged from the chain via a *re-org* (When the fork is reconciled and a single fork turns canonical), the transation may be re-queued for another block. Attackers can leverage these changes to modify the transaction behavior or cancel the transaction based on which fork.

- **Probabilistic finality**: You'll never know when it's finished, it's probably finished in some time in the future but it's not garenteed.

- **Provable Finality**: All blocks published by the network are immediately provably final by definition

