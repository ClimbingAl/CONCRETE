---
title: Data Security
parent: Security, risk, and trust
nav_order: 3
has_toc: false
---

# Data security
{: .fs-9 .no_toc }


Introducing Boss-Based Access Control
{: .fs-6 .fw-300 }
----

This is about risks associated with data (we've covered access to information).  Again we find that Technical tools such as encryption etc that are already used as tools to protect the most secret secrets,  but who has access, who decides.. socio, risk, and trust.  Subtle socio- differences in approach could make for enormous differences in outcomes. The most important of these is to recognise that Data responsibilities are great, but the concept of data ownership in an organisation is an evil capability killer (people can have a data-related responsibility without the need to 'own' it).

Most people for most of the time do not access raw data directly, 
People do When making new tools or are conducting an analytical task.
For most others.
often use software as an intermediary -  transformation for human senses.  visualisation of some sort. whether that's text on a page, a sound, or ..
Access to data going into that software (inputs, or configuration)
when bosses are choosing which data a person can link to.
We have already seen (access-control) that we can control in very fine detail (should we wish) who is accessing what where.



Describe BBAC approach footnote (while this follows the ABAC, RBAC naming scheme, this is a very different, this can be used in distributed decentralised environments and is generally more useful and powerful beast because of the socio- approach aligning with how users manage risk)

This description starts with the concept of potential information content.

- TOC
{:toc}

## Potential information content

![Diagram showing how data about the position of nuclear submarines can be modified or synthesised to reduce the potential information content](../../../../../images/current/potential_information_content.png)


## Data sources and risks

Narrowest data.  Storage and point-to-point.
Aggregation

IPFS
immutability in the storage layer - implications - there are no real modification problems.
To info.

Point to point, but then it's a function of the software too.

Giving somebody access to data where there is an inappropriate level of risk is not a security breach in itself.  It is only when that person subsequently does something like turn it into information and then does something with that, that it becomes a breach.

## BBAC

Principles

It is not your data, it is the King's data.

You cannot self-authorise access to data.


Data meta data tags

- All data is available to users.
- Access decisions are made by ‘boss’ characters.  
- There are no other embedded access rules / processes.
- Users are expected to choose to use datasets that have the minimum possible information content for their task.
- Users are expected to self-impose the most restrictive conditions for that access - including delaying the first access time.
- Meta-data notes help users to understand the risks associated with using a dataset.  
- People can always 'phone a friend' to ask for more opinion 
- Everyone can add to this meta-data guidance including providing links to alternatives.
- Everyone can add tools that enable possible information content to be reduced.
- Everyone can add alternative datasets.
- Requests to bosses and their responses are logged.  
- Access logs are used by counter-intelligence personnel (and systems) to monitor for inappropriate access permissions.
- Bosses might be a direct superior, but they can also come from different roles eg a C2 controller (bosses need to be assigned permissions / capabilities). 
- It is up to bosses to decide whether the correct risk/reward balance is being made.
- A boss granting access to a user does not give themselves an access right.

People interested in data access to a particular data set can always monitor it.  They would be accessing another datastream of course though, which would itself have risk/reward implications.

Guards to monitor and in extreme cases intervene.

Guards nudge both ways - not taking enough risk.  There's a spectrum of risk.  

Guard tooling similar to fraud detection - outliers vs outlaws; trends etc.

## Trust

Honoring the meta-data implications - limit to CONCRETE-enclave size.
Trust boundaries
From small beginnings - group trust dynamics.

Normal to have human cliques, but don't confuse these with organisational lack of trust.  It's all one big team.  

CONCRETE enclave identity is closely related to the IOTA genesis.
## Dynamic risk management

Local-first decision making.  Can't pre-emptively make rules for every situation.

Risks and rewards change over time.

Accelerating by Left-shifting the generation of the information required by data access decision makers to make it available when it's needed.

HQDM - it keeps on appearing :-)


## Responsibilities not ownership

Why data ownership is evil

## Gateways

Gateways are a necessary evil - they are a form of ownership.
At least minimise the effects.
CONCRETE enables people to set up access approaches for people outside their CONCRETE-enclave.  This can be dynamic / rules-based - not just 'have this data'
Also gateways are not just about getting a dataset.
Could compute within a concrete enclave.
May be the case that this could be easier.
CONCRETE-enclave to CONCRETE-enclave boundaries are much easier for everyone.
FHE
We can monitor what's going on.

## Accessing the data behind a piece of information

Accessing information as data - automatic entry in the meta-data associated with information.  Therefore this should flash a big red light with the guards.  Probably want special mechanisms.  May wish to have a guard automation that pauses this.

## Big-bosses

Some consideration required for people at the very top of hierarchies.  Peer-to-peer and/or even specialist groups.
Build in the tools to enable flexible hierarchies of any shape - don't build it in to the foundation.


