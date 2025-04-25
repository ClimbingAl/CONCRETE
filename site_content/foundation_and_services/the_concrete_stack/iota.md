---
title: IOTA
parent: The CONCRETE stack
nav_order: 5
---

# IOTA 
{: .fs-9 .no_toc }


A distributed decentralised ledger
{: .fs-6 .fw-300 }
----
[![iota icon](../../../../images/current/iota_icon.png)](https://www.iota.org/)


IOTA generates a single shared digital ledger (or database) across all nodes.  

<span>Stable</span>{: .label .label-green } Basic IOTA functionality within CONCRETE, as described here, is considered to be stable. Despite this, further work is known to be required to cohere this as part of a wider, performant, CONCRETE whole (LINK).

## Table of contents
{: .no_toc }

1. TOC
{:toc}

## IOTA overview

[IOTA](https://www.iota.org/) is a common piece of software that is run on all (or many[^bft]) nodes.  This software tracks and updates a single shared [^replicated] ledger, or database. A legitimate update, or transaction, requested by a user at node A (below) will eventually be recognised and replicated across the entire network. One of the key features of this (and other distributed ledgers such as Bitcoin, and Ethereum) is that consensus is maintained as a single source of 'truth' despite the potential for failures and hostile actors.

[^bft]:
    Increasing the number of (trustworthy) nodes running this software in a network improves performance and overall security (see wikipedia: [Byzantine fault tolerance](https://en.wikipedia.org/wiki/Byzantine_fault#), for an introduction to some of the security aspects of this).  

[^replicated]:
    Each full IOTA software node holds its own copy of the entire ledger.  There will always be some slight disparities between these nodes (if nothing else, this is a function of physics and the time it takes for information to pass around a network).  However, the algorithms used generate a form of guarantee of eventual consistency.  

![network of nodes each running an instance of iota](../../../../images/current/lettered_nodes_with_iota.png)

IOTA software, like other distributed ledgers technologies such as Bitcoin, use cryptographic (mathematical) techniques[^crypto-strength] to:

- Ensure that certain actions can only be conducted by authorised users.
- 'Mint' unforgeable tokens with similar characteristics to physical money eg they can only be owned by one person at a time.
- Enable 'smart' contracts to automate actions that cannot be tampered with, or be ignored by the parties involved.
- Store data that can only be modified by specific users.

[^crypto-strength]:
    The strength of these cryptographic techniques is important.  As is the quality of the software that is used to instantiate them. The mathematical techniques here are well-researched, and are already future-proofed against the potential for quantum computer attacks (should these ever materialise in practice). The inclusion of seL4 and trusted hardware in the CONCRETE stack will enable developers to formally, mathematically, prove properties about CONCRETE-IOTA-style functionality, rather than leaving any of this to engineering good practice.

IOTA-style functionality has many potential uses in CONCRETE.

## IOTA and identity

User digital identities will be defined in CONCRETE by a private cryptographic key (a large, secret, number) used within IOTA.  Although these keys will be used extensively, users will not be handling them on a day-to-day basis (these will primarily be used 'under-the-hood').  Beyond their primary identity, users will regularly be using cryptographic pseudonyms. These are useful, for example, for security, to ensure that Alice-1 and Alice-2 can be given different permissions by different 'boss' characters without the potential for Alice to aggregate and mis-use combined privileges. 

Various identity-related services can be expected in a CONCRETE-world.  The security of a CONCRETE network will be closely aligned with the security associated with these secret keys. Although this is a well-understood field, there are various layered security approaches to key management to develop.

## IOTA for performant crypto-style tokens in hostile environments

Financial mechanism

Transactions.  Move24.

Security - capability tokens

IOTA and sharding = ABC cut off from rest.

Parallelism

![iota tangle visualised](../../../../images/current/the_IOTA_tangle.png)

## IOTA for naming

Names in general.

HQDM unique identifiers.

## IOTA and trustworthy automations

IOTA for smart contracts.

security - sources of truth.








