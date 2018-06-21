## Decred in Depth: Politeia
### Voice Over

Named after the Greek term meaning ‘a system of government’--Politeia is the Decred proposal system: a chain-anchored social media application where stakeholders decide which projects recieve funding from the network fund. 

Decred governance data hosted on Politeia is made up of submitted project proposals, comments, and up/down votes. 

This user-sourced content is episodically anchored to the Decred blockchain. Censorship tokens allow users to demonstrate when their proposals or comments have been censored.

To achieve this, Politeia's off-chain storage system makes use of Git (a popular revision control system), and DecredTime (a custom server application for storing timestamps on the Decred blockchain).

Git is utilized to create a historic record of every change to the data stored on Politeia. All revisions recorded by Git are anchored to the Decred blockchain through DecredTime. This "Git plus timestamping" equation results in a time sequence of data revisions that is computationally infeasible to recreate.

On the front end, the Politeia GUI provides an easy to use web-based interface for stakeholders to submit project proposals, comments, and votes.

There is a small DCR fee for registering new Politeia accounts (to limit sock-puppets), and for submitting proposals (to limit spam).

Politeia administrators check that proposals conform to basic requirements and either approve them to appear on the public Politeia platform or censor them.

Unlike conventional social media applications, content on Politeia cannot be silently censored. The owner of any content can use their censorship token to prove that it existed in a certain form (and thus, whether it has been censored or edited).

It works like this: once a user submits a proposal for review, they receive a censorship token. After their proposal has been reviewed and deemed in adherence with guidelines, it becomes available for public consideration. When a proposal becomes public, its corresponding censorship token becomes invalid. 

If a stakeholder's proposal is rejected, their censorship token remains valid and can be used to prove that their proposal was censored and identify the administrator responsible. 

The use of censorship tokens in this manner allows stakeholders to hold administrators publicly accountable for their actions.

Cryptographically verifiable and censorship resistant, Politeia is the ideal platform for self-governance. 

To submit your own project proposal through Politeia, download Decrediton at Decred.org and buy Decred on one of the many supporting exchanges.

Decred; Decentralized Credit.
