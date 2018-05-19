## Decred in Depth: Politeia
### Voice Over

### Keywords
`proposal`, `Timestamped`, `versioned`, `self-governance`, `immutable`, `off-chain storage`, `git`, `chain-anchored`

Named after the greek term meaning ‘a system of government’, Politeia is the Decred proposal system: a chain-anchored social media application where Decred stakeholders can take part in deciding which Decred improvement projects recieve funding from the development fund. 

Submitted project proposals, proposal comments, and votes make up Decred's governance data hosted on Politeia. Newly submitted content is episodically anchored to the Decred blockchain creating an immutable and cryptographically verifiable public record of Decred's governance data. Once a proposal is posted to Politeia, the record of its posting can never be altered or deleted, nor can proposals be forged. 

Anchoring Politeia to the blockchain ensures that attempts to manipulate Decred's governance are significantly more difficult than if a traditional website or social media application were in use.

To achieve this chain-anchoring, Politeia's off-chain storage system makes use of Git (a popular revision control system), and DecredTime (a custom server application for storing timestamps on the Decred blockchain.)

Git tracks, hashes, and stores changes to Decred's governance data as revisions to create a historic record of every change to the data stored on Politeia. These revisions are then anchored to the Decred blockchain through DecredTime to construct a time sequence of data revisions that is computationally impossible to recreate.

In order to enforce proposal quality standards and limit the amount of on-chain storage required, proposals submitted through Politeia must be manually reviewed by a human.

In a system where humans must moderate content, censorship is likely to occur. However, content on Politeia cannot be silently censored thanks to a transparent review process made possible by tokens.

Once a user sumbmits a proposal on Politeia for review, they receive a censorship token. After their proposal has been reviewed and deemed in adherence with guidelines, it becomes available for public consideration. Once a proposal becomes public, its corresponding censorship token becomes invalid. However, if a stakeholder's proposal is rejected, their censorship token remains valid and can be used publicly prove that their proposal was censored. The use of censorship tokens in this manner allows stakeholders to hold human administrators publicly responsible for their actions when found to be acting inappropriately.

Politeia is the ideal crytptographically verifiable and censorship resistant platform for self-governance. 

To submit your own project proposal through Politeia, head to decred.org to download the software for your platform and buy Decred on exchanges listed at _decred.org/?_.

Decred; Decentralized Credits.


 	
