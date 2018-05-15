# Decred in Depth: Politeia

### Keywords
`proposal`, `Timestamped`, `versioned`, `self-governance`, `immutable`, `off-chain storage`, `git`, `chain-anchored`

Named after the greek term meaning ‘a system of government’, Politeia is the Decred proposal system: a chain-anchored social media application where Decred stakeholders submit and vote on proposals to spend the development fund. 

Stakeholder proposals, proposal comments, and votes submitted through Politeia are anchored to the blockchain creating an immutable and cryptographically verifiable public record of Decred's governance-data. Once a proposal is posted to Politeia, the record of it's posting can never be altered or deleted, nor can records of proposals be forged. 

Anchoring Politeia to the blockchain ensures that attempts to manipulate Decred's governance are significantly more difficult than if a traditional website or social media application were in use.

To achieve this Politeia's off-chain storage system is a combination of revision control via Git (a popular revision control system), and cryptographic timestamping via DecredTime (a custom server application for storing timestamps on the Decred blockchain.)

Git tracks, hashes, and stores changes to Decred's governance data as revisions. These stored revisions make up the public record of Decred governance on Politeia. DecredTime then takes the hashes of these revisions, and anchors them to the Decred blockchain creating a time sequence that is computationally impossible to recreate.

Fancy programming alone cannot create a perfect self-governance system. In order to enforce proposal quality standards and limit the amount of on-chain storage required, proposals submitted through Politeia must be manually reviewed by a human.

Where there are humans there is bias. Where there is bias, there is often censorship.

It is not possible to eliminate censorship in a system where humans must decide which media is approved for public viewing. However, by making use of a censorship token, silent censorship becomes impossible.

Once a proposal is submitted, it is classified as ‘unvetted’ and the stakeholder who submitted the proposal receives a censorship token. After a proposal has been reviewed and deemed in adherence with proposal guidelines by a human administrator, it's labeled ‘vetted’ and becomes available for public consideration. Once a proposal becomes vetted, it's corresponding censorship token becomes invalid. If a proposal is rejected by an administrator, the stakeholder holding the corresponding censorship token to publicly prove their proposal was censored. Censorship tokens, create a transparent review process where administrators can be held publicly responsible for their actions when found to be acting inappropriately.

Politeia is the ideal infrastructure for self-governance of a crypto-currency. To contribute to Decred’s governance, head to decred.org to download the software for your platform and buy decred on exchanges such as bittrex and poloniex.

Decred; Decentralized Credits.


 	
