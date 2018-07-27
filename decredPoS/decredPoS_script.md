## Decred In Depth: Stake Voting
### Voice Over Script

Decred proof-of-stake is an on-chain decision making system where participants purchase tickets for a chance to have their voice heard.

To purchase a ticket, participants must have enough Decred to cover the current ticket price.

Every 144 blocks, a new ticket price is calculated by a pricing algorithm to keep the total number of active tickets equal to the target size.

If the participant's balance is high enough, a portion equal to the current ticket price may be locked in exchange for a ticket. Locke funds cannot be spent for the duration of the ticket lifecycle. The exact length of a specific ticket's life is largely up to chance, but averages 30 days.

A ticket's life begins after it is mined into a block. How long a ticket must wait to be mined is determined by the ticket fee paid when it was purchased. Once included in a block, a ticket is considered immature and must wait about 12 hours before it becomes live and is added to the ticket pool.

The ticket pool is where live tickets wait to be chosen to vote. Every 5 minutes, using arbitrary entropy from the blockchain, 5 tickets are randomly drawn from the pool to cast their votes.

Once their ticket is drawn, a participant's votes are broadcast to the network by their chosen stake voting service for inclusion in the next block.

There are two on-chain voting process to participate in: block votes and consensus votes.

Block votes provide a mechanism for participants to keep non-conforming proof-of-work miners in check. 5 votes in each new block decide whether to reject the previous block. If the block is rejected, the founding miner will not receive their part of the block reward.

Consensus voting is a two stage process where participants vote for or against the implementation of changes to the Decred network. If enough nodes upgrade within the upgrade phase interval, voting commences. If 75% of votes signal yes within the voting interval, then the changes are ratified and will be automatically implemented after another block interval.

After a participant's block and consensus votes have been cast, the funds used to purchase the ticket are unlocked and a portion of the block reward is credited to their account.

Other decisions not involving consensus rule changes, such as how to spend the project subsidy fund, are decided through Politeia, the Decred proposal system. Through their wallet, participants with live tickets can vote to approve or deny Politeia proposals.

To begin participating in Decred proof-of-stake, download Decrediton at Decred.org and purchase Decred at any one of the many supporting exchanges.

Decred; Decentralized Credits.