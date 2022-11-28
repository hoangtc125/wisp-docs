---
sidebar_position: 3
---

Proposals & Voting
==================

The Wisp DAO governance process takes place in the governance forum at [forum.wispswap.io](http://forum.wispswap.io). Proposals are formally ratified through the Wisp Improvement Proposal (WIPs). There are no requirements for participating in the Wisp DAO discussion. Anyone can sign up for the 1inch Governance forum, or Discord and engage in the conversation.

### 

Phase 1: Discussion[](#phase-1-discussion)

The purpose of this phase is to vet ideas with the broader 1inch community. Each unique idea should have its own thread so that the conversation can stay on topic, it should be as narrowly focused as possible. Anyone can participate in this phase of governance, and it occurs entirely off-chain. The goal of Phase 1 discussion is to gain a rough community consensus, and refine the idea so that it can be formalized. The thread author should make an effort to address all comments and take them into consideration.

### 

Phase 2: Formalization[](#phase-2-formalization)

Phase 2 is where the idea is formalized into an WIP that includes all of the criteria. It must be a clear and complete description of the proposed enhancement. It is a requirement that a single WIP contains a single proposal.

The forum is the formal arena to debate the merits of each WIP. Once the WIP has been drafted, the author must post it on the WispSwap governance forum and use tag `phase-2`

While the WIP is in a draft state, the WIP author is free to make modifications to the proposal based on feedback from the community's review.

To preserve the number sequencing of WIPs, proposals should use the RC (Request for Comment) prefix for both Phase 2 and Phase 3. The WIP number will be assigned once the proposal enters the Phase-4 Snapshot vote.

### 

Phase 3: Temperature Check[](#phase-3-temperature-check)

At any point during Phase 2, the author may finalize the WIP by initiating a community temperature check. To do this, the author must change the tag of the forum post to `phase-3`, and add a forum poll to gauge the community’s sentiment.

WIPs should only be progressed to Phase 3 once the author has considered all community comments and believes the WIP is prepared for incorporation. Phase 3 represents the final proposal. Other than correcting errata, WIPs in Phase 3 may not be edited.

The poll must be open for 5 days and only have the following options:

*   (Yes) In favor of this proposal.
    

*   (No) Against this proposal.
    

Only successful Phase 3 proposals may progress to Phase 4. In order for a Phase 3 vote to be considered successful, a majority of the temperature check votes cast must be in favor. There is no minimum quorum required for this phase.

### 

Phase 4: Snapshot Vote[](#phase-4-snapshot-vote)

All WIPs are confirmed, or rejected, by the WispSwap DAO via an off-chain Snapshot vote. The Snapshot vote must link to the results of the successful Phase-3 forum poll and include the full text of the finalized WIP. Anyone can initiate the Snapshot vote as long as all requirements of Phase-3 were met. Once the Snapshot vote has been created, the forum tag should be changed to phase-4.

The Snapshot voting period must last exactly seven days. During this period, addresses with voting power may vote for or against the proposal using the same two voting options as the Phase 3 poll:

*   (Yes) In favor of this proposal.
    

*   (No) Against this proposal.
    

There will be an automatic **snapshot** of wallets _everyday_. The snapshot will capture the amount of WISP, the WISP in WISP-SUI LP Tokens, the WISP in WISP-SUI LP in Yield Farming and the WISP in the staking system in anyone’s wallets. It's not necessary to unstake LP Tokens to access snapshot voting.

**Voting Power** will be the same for WISP regardless of whether it is liquid, in LP or staked.

**Quorum** is the metric which requires the minimum of unique Voting Power of each proposal. If the proposal has the unique Voting Power less than Quorum, then the proposal won’t be approved. For a vote to pass and become binding, it must gain a quorum of at least **5% of the current $WISP circulating supply** (subject to changes).

### 

Phase 5: Implementation[](#phase-5-implementation)

After the Snapshot voting period has concluded, the results will be posted on WIPs section of the governance documentation site. If the proposal has passed, it will move from the Active to Passed category. Unsuccessful proposals will move to Not-Passed.