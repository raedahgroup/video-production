#Decred in Depth: Politeia

### Keywords
`proposal`, `Timestamped`, `versioned`, `self-governance`, `immutable`, `off-chain storage`, `git`, `chain-anchored`

Named after the greek term meaning ‘a system of government’, Politeia is the Decred proposal system a social media application where Decred stakeholders submit proposals for projects to upgrade and market the Decred network. 

Politeia is special in that it is designed to be an immutable and cryptographically verifiable public record of Decred’s governance-data. This means that once a proposal is posted to Politeia, the record of that proposal’s posting can never be altered or deleted. In addition, records of proposals cannot be forged. The time ordered and independently verifiable nature of Politeia ensures that attempts to manipulate Decred’s governance are significantly more difficult than if a traditional website or social media application were in use.

From a technical standpoint, Politeia is an off-chain storage system comprised  of Git, a popular revision control system, and cryptographic timestamping via DecredTime, a custom server application for storing timestamps on the Decred blockchain.

Git tracks and stores changes to Politeia as revisions. These stored revisions make up the public record of Decred governance on Politeia. DecredTime takes unique identifiers of these revisions, called hashes, and anchors them to the Decred blockchain, creating a time sequence that is computationally impossible to recreate.

Like reddit, content posted to Politeia must be manually reviewed by a human. This presents a problem common to all social media today: silent censorship. Politeia has a system in place to deal with censorship. 

It works like this:

Once a proposal is submitted, it is classified as ‘unvetted’ and the user who submitted the proposal receives a censorship token. After the proposal has been reviewed and deemed in adherence with proposal guidelines, it is considered ‘vetted’ and becomes available for public viewing. When a proposal becomes vetted, the corresponding censorship token is no longer valid. If a proposal never becomes vetted, the proposal submitter can use their censorship token to publicly prove their proposal was censored. By using censorship tokens, politeia creates a transparent censorship process. Administrators can be held publicly responsible for their actions when found to be acting inappropriately.

Politeia is the ideal infrastructure for self-governance of a crypto-currency. To contribute to Decred’s governance, head to decred.org to download the software for your platform and buy decred on exchanges such as bittrex and poloniex.

Decred, Decentralized Credits.


 	
