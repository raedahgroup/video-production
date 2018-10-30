## Decred In Depth: Proof-of-stake Voting

### Storyboard
**Estimated Runtime:**

| No. | VISUAL | DESCRIPTION | TIME |
| :-: | :----: | :---- | :--: |
| 1 |  | Thumbnail |  |  |
| 2 | ![shot 2](../decredPoS/img/shot_2.svg)? | **VO**:<br />Without a form of on-chain governance, pure proof-of-work currencies like Bitcoin are at the mercy of their miners. With no way to keep proof-of-work miners in check *or* agree on consensus rule changes,<br />**action**:<br /> |  |
| 3 | ![shot 3](../decredPoS/img/shot_3.svg) | **VO**:<br />these currencies leave themselves open to 51% attacks and chain-splitting hard forks.<br />**action**:<br /> |  |
| 4 | ![shot 4](../decredPoS/img/shot_4.svg) | ****VO**:<br />Decred's** **Proof-of-Stake Voting** system, (which is part of its hybrid proof-of-work - proof-of-stake protocol),<br />**action**:<br /> |  |  
| 5 | ![shot 5](../decredPoS/img/shot_5.svg)? | **VO**:<br />puts power in the hands of its stakeholders, not its miners.<br />**action**:<br />stakeholder becomes larger than miner |  |
| 6 | ![shot 6](../decredPoS/img/shot_6.svg) | **VO**:<br />By participating in proof-of-stake voting, stakeholders can stop 51% attacks, prevent unwanted hard forks, and shape the future of the project.<br />**action**:<br /> |  |  
| 7 | transition | **VO**:<br />Here's how it works:<br />**action**:<br /> |  |
| 8 | ? | **VO**:<br />Decred Proof-of-stake voting is a ticket-based lottery system.<br />**action**:<br /> |  |  
| 9 | ![shot 9](../decredPoS/img/shot_9.svg) | **VO**:<br />Stakeholders prove their stake by time-locking funds in exchange for tickets.<br />**action**:<br />dcr funds locked and ticket dispensed |  |  
| 10 | ![shot 10](../decredPoS/img/shot_10.svg) | **VO**:<br />Each ticket owned offers a chance to participate in the governance of the project by casting votes.<br />**action**:<br /> |  |
| 11 | ![shot 11](../decredPoS/img/shot_11.svg)stepped Graph showing ratio of dcr owned to potential # of tickets | **VO**:<br />The more tickets a stakeholder can acquire the more votes they can cast.<br />**action**:<br /> |  |  
| 12 | ![shot 12](../decredPoS/img/shot_12.svg)Graph of ticket price over time. **Text:** (144 blocks * 5) / 60 = ~12 hours | **VO**:<br />The *price* of a ticket is automatically adjusted by an algorithm at the end of each **ticket window** of 144 blocks; (about 12 hours, given Decred's average **block time** of roughly 5 minutes.)<br />**action**:<br /> |  |  
| 13 | ![shot 13](../decredPoS/img/shot_13.svg)Graph of ticket pool size over time | **VO**:<br />This keeps the number of *live* tickets in the system as close as possible to the target 40,960 tickets.<br />**action**:<br /> |  |
| 14 | ![shot 14](../decredPoS/img/shot_14.svg) | **VO**:<br />A ticket's life *begins* when it is first mined into a block, and *ends* when it is drawn from the ticket pool.<br />**action**:<br /> |  |
| 15 | ![shot 15](../decredPoS/img/shot_15.svg) | **VO**:<br />Before it is added to the ticket pool, a ticket must go through the immature stage. During this stage, the stakeholder's funds used to acquire the ticket are locked, but the ticket is not yet eligible to be drawn.<br />**action**:<br /> |  |  
| 16 | ![shot 16](../decredPoS/img/shot_16.svg) | **VO**:<br />After 256 blocks (or about 21 hours), immature tickets become live and are added to the **ticket pool**.<br />**action**:<br /> |  |
| 17 | ? | **VO**:<br />With each block, 5 tickets are randomly drawn from the ticket pool.<br />**action**:<br /> |  |
| 18 | ![shot 18](../decredPoS/img/shot_18.svg) | **VO**:<br />How long an individual ticket will wait in the pool before being drawn is entirely up to chance, but the average waiting time is close to one month.<br />**action**:<br /> |  |  
| 19 | ![shot 19](../decredPoS/img/shot_19.svg) | **VO**:<br />In rare circumstances, it is possible for a ticket to never be drawn. This occurs with less than 1 percent of all tickets and results in a full refund of the expired ticket's price.<br />**action**:<br /> |  |  
| 20 | ![shot 20](../decredPoS/img/shot_20.svg) | **VO**:<br />Once their ticket is drawn, a ticketholder's votes must be broadcast to the network from either their own *self-hosted* **voting wallet** or a designated **voting service provider** for inclusion the next block.<br />**action**:<br /> |  |  
| 21 | ![shot 21](../decredPoS/img/shot_21.svg) | **VO**:<br />If votes are not broadcast quickly enough, their intended block may be mined without them. This occurs in less than 2% of cases and results in a full refund of the missed ticket's price.<br />**action**:<br /> |  |
| 22 | ![shot 22](../decredPoS/img/shot_22.svg) | **VO**:<br />For each drawn ticket, a ticketholder may cast one **block vote** and zero to many **consensus votes** to be recorded *on-chain*.<br />**action**:<br /> |  |
| 23 | scale? | **VO**:<br />Block votes allow ticketholders to keep proof-of-work miners in check.<br />**action**:<br /> |  |
| 24 | ![shot 6](../decredPoS/img/shot_24.svg)technical diagram of a block | **VO**:<br />The 5 block votes contained in each new block decide whether to accept or reject the previous one.<br />**action**:<br />block votes 'reject' block |  |  
| 25 | 1s![shot 25](../decredPoS/img/shot_25.svg) | **VO**:<br />If stakeholders decide to reject the block, its regular transactions are returned to the mempool and the miner is stripped of their block reward.<br />**action**:<br /> |  |
| 26 | ![shot 26](../decredPoS/img/shot_26.svg) | **VO**:<br />Consensus votes allow ticketholders to prevent unwanted hard-forks through a two stage process where stakeholders vote for or against changes to Decred's consensus rules.<br />**action**:<br /> |  |  
| 27 | ? | **VO**:<br />Before the consensus voting process can begin, a majority of nodes must update to the newly released software version containing the dormant rule change.<br />**action**:<br /> |  |
| 28 | ![shot 28](../decredPoS/img/shot_28.svg) | **VO**:<br />The update threshold is met when 95% of the 1000 most recent blocks were found by updated miners and 75% of the proof of stake votes within *one* **stake version interval**, 2016 blocks (or about 1 week), were cast by updated voting wallets.<br />**action**:<br /> |  |  
| 29 | ![shot 29](../decredPoS/img/shot_29.svg) | **VO**:<br />After the update threshold is met voting will begin on the *first block* of the next **rule change interval**.<br />**action**:<br />SVI blocks are added one by one |  |
| 30 | ![shot 30](../decredPoS/img/shot_30.svg) | **VO**:<br />Each rule change interval spans 8,064 blocks (or about 4 weeks) during which votes for any active rule change processes are collected.<br />**action**:<br />SVI's continue to be added. The last block is added then the timeline slides to the left to make room for the next RCI |  |  
| 31 | ![shot 31](../decredPoS/img/shot_31.svg) | **VO**:<br />A revote occurs if 90% of votes collected during the entire interval abstain.<br />**action**:<br /> |  |
| 32 | ![shot 32](../decredPoS/img/shot_32.svg) | **VO**:<br />Else, if 75% of non-abstaining votes signal yes, then the proposed rule changes will be activated at the end of the *next* rule change interval.<br />**action**:<br /> |  |  
| 33 | ![shot 33](../decredPoS/img/shot_33.svg) | **VO**:<br />After a ticketholder's votes has been included in a block and another immaturity phase has passed,<br />**action**:<br /> |  |
| 34 | ![shot 34](../decredPoS/img/shot_34.svg) | **VO**:<br />the price of the voted ticket is fully refunded and a portion of the Decred block reward is credited to their account as compensation for their active participation.<br />**action**:<br /> |  |  
| 35 | ![shot 35](../decredPoS/img/shot_35.svg) | **VO**:<br />On-chain voting allows stakeholders to govern the chain, but what about governance of the project itself?<br />**action**:<br /> |  |
| 36 | ![shot 36](../decredPoS/img/shot_36.svg) | **VO**:<br />While their live tickets are waiting in the ticket pool, ticketholders have access to proposal voting through Politeia, Decred's chain-anchored proposal system.<br />**action**:<br /> |  |  
| 37 | pi mockup with example proposals | **VO**:<br />Through Politeia anyone can shape the future of Decred by proposing new ideas for stakeholder consideration in an off-chain yet cryptographically verifiable manner.<br />**action**:<br /> |  |
| 38 | ![shot 38](../decredPoS/img/shot_38.svg) | **VO**:<br />To begin participating in the governance of Decred, download Decrediton at Decred.org<br />**action**:<br /> |  |
| 39 | ![shot 39](../decredPoS/img/shot_39.svg) |**VO**:<br />and purchase Decred at any one of the many supporting exchanges.<br />**action**:<br />|  |
| 40 | ![shot 40](../decredPoS/img/shot_40.svg) | **VO**:<br />Decred; Decentralized credits.<br />**action**:<br /> |  |
| 41 |  | End-card |  |