# Decred In Depth: Stake Voting

### Keywords
    unique, lucrative, investor, stake vote, no effort, risk-free, proof-of-stake

Decred’s unique stake voting system offers a functional and lucrative opportunity to investors. By participating in the proof-of-stake mining system, investors become stake voters helping to both secure the Decred blockchain and choose the direction of its evolution.

Investors can become stake voters and begin earning Decred at 15% APR with zero risk by purchasing tickets.

In order to purchase a ticket, an investor must lock an amount of their coins equal to the ticket price for the life of the ticket.

The ticket price is a variable figure based on the number of tickets waiting to be drawn in what is called the ticket pool. The ticket price is automatically adjusted to keep the size of the ticket pool stable. If the ticket pool contains more than the optimum 40,960 tickets, the price to purchase a ticket will be increased. This discourages ticket buying and allows time for the ticket pool to return to the optimal ticket count. If there are too few tickets in the ticket pool, the price will be lowered in order to kickstart ticket buying.

The order in which tickets are chosen to vote is determined randomly, similar to a lottery drawing. Once per block *(?)*, using random numbers from the previous block, the blockchain will draw 5 tickets from the ticket pool.
Each ticket in the ticket pool has a 99.5% chance of being drawn within 5 months. On average, a ticket will wait in the pool for 30 days. For the 0.5% of tickets that expire, the purchasing funds are unlocked and can be used to purchase a replacement ticket.

When a ticket is drawn, its votes are mined into a block. The 5 total ticket votes in each block serve two functions.

First, each ticket votes on the validity of the last seen block. If a block is deemed invalid by at least a 3 to 5 majority, then the entire block is invalidated except for the proof-of-stake portion of the block reward. This means that the proof-of-work reward and the transactions are stripped from the network. This process acts as a check on miner power, giving stakeholders a way to crack down on miners who are not following the rules and prevent 51% attacks.

Secondly, a ticket may cast `yes`, `no`, or `abstain` votes concerning upgrade proposals submitted by stakeholders through Politeia; Decred’s proposal system.
If a specific proposed update receives the required number of `yes` votes, it is collectively implemented by the network and upgrades the consensus rules of the chain. This process puts the power to decide the future of Decred in the hands of stakeholders and prevents potentially troublesome chain splits.
Once a ticket has voted, the Decred spent to purchase the ticket is unlocked and a reward for voting, called a ticket reward, is deposited in the ticket owners account. This ticket reward amounts to 6% of the total decred block reward. After a waiting period of 20 hours, these funds are available to be spent on additional tickets.

Stake voting requires no action by the stakeholder other than purchasing tickets. By default, tickets are configured to abstain from voting on upgrade proposals, however `yes` or `no` votes can be configured easily through the Decrediton staking wallet.

In order to ensure that a vote is not missed, a stake server can be used.
Stake servers allow stake voters to cast votes without worrying about missed votes due to computer downtime, bad internet connections, or inconsistent electricity grids.

Stake servers will vote on behalf of a stake voter for a small fee. This server fee helps pay for the cost of server infrastructure needed to ensure tickets vote quickly and reliably.

In rare cases, it is possible for votes to be missed even though they were cast. This can happen when miners are processing blocks faster than the votes can propagate through the network.

Miners are incentivised to include the ideal 5 votes per block, but are only required to include the necessary minimum of 3 votes. A miner may only include 3 votes in a block *for some reason (can't seem to find explanation why this may happen)*. If this is the case and a block is mined with only 3 votes, the remaining 2 votes destined for that block are considered ‘missed’ and the funds used to purchase them are unlocked.
To estimate the amount of Decred a stake voter can earn in a year through proof of stake mining, use this equation to calculate the annual percentage rate.

`(ticket reward / ticket price) / ticket lifespan [in years] = Annual Percentage Rate` ( *not sure if this is the correct equation* )

Assuming, for example, a ticket reward of 1.3 Decred, a ticket price of 88 Decred, and using the average ticket lifespan of 30 days (or 0.082 years), the annual percentage rate if 1 ticket is purchased at a time works out to 18%.

Best of all, that 18% comes risk free; staked coins never leave your wallet and are always unlocked after a ticket either expires, votes, or misses.

To begin earning your own ticket rewards, download decrediton for your 
platform at decred.org and click on the tickets tab.

Decred, Decentralized Credits
