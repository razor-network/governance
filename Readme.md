# Razor Network Governance Handbook

**Disclaimer**: The governance is currently in its bootstrapping phase, with the governance strategies still under beta. Thus, guidelines are subject to change at any given moment. Additionally, even if proposed, particular suggestions might not be implemented if they are considered detrimental to the protocol.

## Objective

This handbook provides direction on how to govern the parameters of the Razor Network—a decentralized oracle network. Note that the governance will be progressively decentralized, with various protocol components transitioning to decentralized governance over time.

Governance Mechanism's Scope:

- Datafeeds and Collections

## General Information

- **Where to Propose**: [Submit Proposals Here](https://snapshot.org/#/raz.eth)
- **Voting Delay**: 2 days
- **Voting Period**: 7 days
- **Quorum**: 100M 

### Governance Flow:

1. If needed, initiate a Pull Request in the appropriate repository.
2. Start a discussion thread at [Razor Network Governance Discussions](https://github.com/razor-network/governance/discussions).
3. Draft a proposal and include links to the PR and the discussion thread.
4. Update the discussion thread and PR, adding a link to the finalized proposal.

## Eligibility Criteria

### Voting

- Eligible Voters: All RAZOR token holders on the Polygon mainnet and Ethereum mainnet. 
- Razor network validators and delegators are also eligible to vote. They must vote with the address holding sRZR. Their voting power equates to the number of equivalent RAZOR tokens they hold.
- Minimum Tokens for Voting: Currently, no minimum. 

### Proposals

- At present, only authors are permitted to draft proposals. Future outlook: Individuals with a specific minimum voting power can create a proposal.
- Submit a governance proposal at [Proposal Submission Portal](https://snapshot.org/#/raz.eth).
- Proposals should fall within specified categories and meet the pertinent criteria.

## Data Sources

### Datafeeds

Governance can add or remove data feeds based on votes. Requirements for a valid data feed:

- API must be accessible to the public.
- The endpoint should exhibit stability, with minimal errors.
- API call limits should be ample. 1 Request per 10 minutes at the minimum, from the same IP address. (Razor network currently makes one request every 20 minutes)
- API responses should be in JSON or XHTML formats.
- The feed should be available across all geographical regions.
- It must clear specific tests.

### Collections

A collection refers to an amalgamation of data feeds specific to a particular dataset. Key characteristics of collections:

- Should comprise a minimum of 5 and a maximum of 10 data feeds.
- All data feeds within a collection must be interrelated.
- The power metric used should be uniform.
- The collection must pass designated tests.

**Note**: Proposals can request the addition or removal of a single collection at a time.

### Proposal Documentation

For Datafeeds or Collections proposals, draft a PR at [Razor Network Datasources](https://github.com/razor-network/datasources) and include the link to this PR in the proposal documentation.

[Further Reading on Data Feed and Collection Parameters](LINK TO DOCS).
