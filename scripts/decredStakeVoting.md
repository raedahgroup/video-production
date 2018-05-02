# Decred In Depth: Stake Voting

### Keywords
`unique`, `lucrative`, `investor`, `stake vote`, `no effort`, `risk-free`, `proof-of-stake`

Decred’s unique stake voting system offers a functional and lucrative opportunity to investors. By participating in the proof-of-stake mining system, investors become stake voters helping to both secure the Decred blockchain and choose the direction of its evolution.

Investors can become stake voters and begin earning Decred at 15% APR with zero risk by purchasing tickets.

By purchasing a ticket, an investor locks a portion of their Decred funds equal to the current ticket price.

The price of a ticket varies based on the number of tickets waiting in what is called the ticket pool. Ticket price is automatically adjusted to keep the size of the ticket pool stable. If the ticket pool contains more than the optimum 40,960 tickets, the price to purchase a ticket will increase. An increased ticket price will discourage ticket buying. A discouraged ticket market will allow the number of tickets in the pool to shrink. If there are too few tickets in the ticket pool, the price will decrease to kick-start investment and grow the pool.

A ticket in the pool has a 99.5% chance of being drawn within 5 months. On average, a ticket will only wait in the pool for 30 days. For the fraction of a percent of tickets that expire, the corresponding staked Decred are unlocked, ready to be spent on a replacement ticket.

Tickets that are drawn from the pool are chosen randomly. Using random entropy from the blockchain, 5 tickets are drawn.

When a ticket is drawn, it's owner's vote will be cast by their configured stake server.

Stake servers allow the casting of votes without worry of losses due to computer downtime or bad Internet connections. In return, stake servers receive a small fee taken from vote proceeds. This server fee helps pay for the cost of server infrastructure needed to ensure stake votes are cast quickly and reliably.

The 5 stake votes contained in each new block vote on the validity of the previous one. If this block is deemed invalid by at least a 3 to 5 majority, then its associated transactions and proof-of-work reward are stripped from the network while the proof-of-stake reward is retained. This process acts as a check on miner power, giving stakeholders a way to crack down on miners who are not following the rules and prevent miner aggressions such as block withholding or a 51% attack.

A ticket may also cast votes concerning other agenda items put up for a community vote. One example of an item that was approved in this manner was a consensus rule upgrade improving the algorithm which sets ticket price.

In rare cases, it is possible for votes to be missed even though they were cast. This can happen when miners are processing blocks faster than the votes can propagate through the network. This leads to the mining of blocks with less than 5 votes. If a block is mined with less than the required 5 votes, the remaining votes destined for that block are considered ‘missed’ and the funds used to purchase them are unlocked.

After a stake voter's ticket has been drawn and their votes are successfully cast, the Decred spent on the ticket is unlocked and a reward for voting, called a ticket reward, is deposited into the ticket owners account. This ticket reward amounts to 6% of the total Decred block reward. After a waiting period of 20 hours, these funds become available for spending.

Stake voting requires no action by the stakeholder other than purchasing tickets. By default, tickets are configured to `abstain` from voting on current agenda items, however, `yes` or `no` votes can be configured easily through the Decrediton staking wallet.

Decrediton uses cryptographic ticket "receipts" to verify and allow stake voters to interface with Politeia; Decred's chain-anchored proposal system. Through Politeia, stake voters can participate in Decred self-governance by proposing issues for the community to vote on and voting on those proposed by others.

By participating in Decred self-governance through the Stake Voting system, investors can earn significant returns.

This equation can be used to calculate the annual percentage rate of returns gained through proof-of-stake mining Decred.

`(ticket reward / ticket price) / ticket lifespan [in years] = Annual Percentage Rate`

Assuming, for example, a ticket reward of 1.3 Decred, a ticket price of 88 Decred, with the average ticket lifespan of 30 days (or 0.082 years), the annual percentage rate of 12 tickets purchased in a year works out to 18%.

Best of all, that 18% comes risk free; staked coins never leave your wallet and are always unlocked after a ticket expires, votes, or misses.

To begin earning your own ticket rewards, download Decrediton for your 
platform at Decred.org and click on the "tickets" tab.

Decred, Decentralized Credits
