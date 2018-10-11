## Decred In Depth: Proof-of-stake Voting
### Voice Over Script

Without a form of on-chain governance, pure proof-of-work currencies like Bitcoin are at the mercy of their miners. With no way to keep proof-of-work miners in check *or* agree to a future direction these currencies leave themselves open to malicious attacks and destructive "hard forks"

**Decred's** utilised a unique hybridised **Proof-of-Work** and **Proof-of-Stake Voting** system putting power back into the hands of currency stakeholders. By participating in proof-of-stake voting, stakeholders can halt network attacks, prevent unwanted hard forks, and shape the future of the project.

Decred Proof-of-stake voting is a ticket-based lottery system.

Stakeholders prove their stake by time-locking funds in exchange for tickets. Each ticket purchased offers an opportunity to participate in the governance of the project by casting votes. The more tickets a stakeholder can acquire the more votes they can cast.

The *price* of a ticket is automatically adjusted by an algorithm at the end of each **ticket window** of 144 blocks; approximately 12 hours.  This keeps the number of *live* tickets in the *ticket pool* as close as possible it's target of 40,960 tickets.

A ticket's life *begins* when it is first mined into a block, and *ends* when it either votes or expires.

Before it is added to the ticket pool, a ticket must go through an immature stage. During this stage, the stakeholder's funds used to acquire the ticket are locked, but the ticket is not yet eligible to be drawn.

After 256 blocks (or about 21 hours), immature tickets become live and are added to the **ticket pool**. 

Approximately every *5 minutes* a block is mined and *5 tickets* are randomly drawn from the ticket pool.

How long an individual ticket will wait in the pool before being drawn is entirely up to chance, but at the target *ticket pool* size the average waiting time is approximately a month. In rare circumstances, it is possible for a ticket to never be drawn. Expired tickets can be *revoked* unlocking the inital funds staked.

Once their ticket is drawn, a stakeholder's votes must be broadcast to the network from either their own *self-hosted* **voting wallet** or a designated **voting service provider** for inclusion the next block. If votes are not broadcast quickly enough, their intended block may be mined without them. Alike an Expired tickets, the funds staked on a Missed ticket can be unlocked. 

For each drawn ticket, a stakeholder may cast one **block vote** and zero to many **consensus votes** to be recorded *on-chain*.

Block votes allow stakeholders to keep proof-of-work miners in check. The 5 block votes contained in each new block decide whether to accept or reject the previous one. If stakeholders decide to reject the block, the miner is stripped of their block reward and its regular transactions are returned to the mempool.

Consensus votes allow stakeholders to prevent unwanted hard-forks through a two stage process where stakeholders vote for or against changes to Decred's consensus rules.

Before the consensus voting process can begin, a majority of nodes must update to the newly released software version containing the dormant rule change. The update threshold is met when 95% of the 1000 most recent blocks were found by updated miners and 75% of the proof of stake votes within *one* **stake version interval**, 2016 blocks (or about 1 week), were cast by updated voting wallets. 

After the update threshold is met voting will begin on the *first block* of the next **rule change interval**. 

Each rule change interval spans 8,064 blocks (or about 4 weeks) during which votes for any active rule change processes are collected.  A revote occurs if 90% of votes collected during the entire interval abstain.  Else, if 75% of non-abstaining votes signal yes, then the proposed rule changes will be activated at the end of the *next* rule change interval.

After a stakeholder's votes has been included in a block and a 256 block immaturity phase has passed, the price of the voted ticket is fully refunded and a portion of the Decred block reward is credited to their account as compensation for their active participation.

On-chain voting allows stakeholders to govern the chain, but what about governance of the project itself?

While their live tickets are waiting in the ticket pool, stakeholders have access to proposal voting through Politeia, Decred's chain-anchored proposal system. Through Politeia anyone can shape the future of Decred by proposing new ideas for stakeholder consideration in an off-chain yet cryptographically verifiable manner.

To begin participating in the governance download Decred's offical wallet Decrediton at Decred.org.

You can up your stake by purchasing decred at any one of the many supporting exchanges.

Decred; Decentralized credits.



