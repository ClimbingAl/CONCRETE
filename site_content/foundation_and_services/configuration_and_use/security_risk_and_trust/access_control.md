---
title: Access Control
parent: Security, risk, and trust
nav_order: 1
has_toc: false
---

# Access Control
{: .fs-9 .no_toc }


Digital permissions
{: .fs-6 .fw-300 }
----

Digital access control, not in the sense of access to building etc - that's talked about here.

The seL4 operating system, that runs every CONCRETE device is built on the concept of 'capabilities'. A capability is a unique unforgeable token that bestows on its possessor specific permission to access or use one or more resources within the system itself (very fine-grained access to sub-components, processes, networking, memory, disks etc).  Importantly,  without a capability token, nothing happens. 

The IOTA distributed ledger enables distributed, decentralised users to configure and mint unique unforgeable tokens that can moved around roughly in the same way we would a physical object such as a serial-numbered bank note.  The socio-technical outline is for all access to all digital resources to be controlled by these IOTA tokens.  Bosses (various - discussed later) provide these tokens to users.  Nothing happens without this authority, or put another way, everything has a golden thread that links back to an original authority.

The main associated software development activities would be to generate two tools: one close to seL4 that translates IOTA tokens into its own capabilities, and a user-facing toolset to enable people to easily construct and manage the IOTA tokens themselves.  

There are many other socio-technical aspects and details:

(Get into IOTA pointer to IPFS information?)


- TOC
{:toc}

## Fine-grained management and pipelines

Programs - uniquely identified.  

Data is uniquely identified.  

Machine components are uniquely identified...

The configuration of a program can be uniquely identified ..

Can be linked with results from other sources - so location, network access..

Pipelines - combining these things together from source data -> process -> output data.

Not necessarily onerous - expect lots of standards permissions for standard things - this is more about giving ourselves the fine control for when we need it.

## Dynamic risk management

Dynamic risk management - Agile combat employment example - we all work in an HQ building until a boss decides to re-locate because of a threat - the boss changes all the permissions of users, in one go, to work from 'anywhere' instead of 'HQ-only' - people relocate.  (Try doing that with current systems.) 

Risk/reward - Local management of risk/reward trade-offs. Ties back to basic user needs.

There can still be leadership and guidance, but there isn't a central 'computer says no' system to re-program in light of ever-changing world events.

This is much more powerful and useful than centralised ABAC/RBAC approaches.

Overall security position is an emergent property of many smaller decisions.

## Auth to auth, revocation, risk management, and guards

We can still monitor the permissions being granted and ,if necessary revoke them.

King

Tokens within tokens.

Off-line, on-line

Guards and who guards the guards.

## The need for pseudonyms

pseudonyms - confused deputy - prevent personnel from combining multiple tokens from different bosses (without them knowing it) to gain a capability that was not envisaged.

Different projects from the same boss.

## HQDM

Semantic clarity.

Not about restricted set of possibilities.

Enable the boss to be precise when they want to be

functionality to be clear about what we can do and what is being asked.

Only use this in room 123. - what do we mean by 'in' and 'room 123'.  We don't want a fragile standardised approach - HQDM enables us to do this.

Doesn't have to be a major burden.

Probabilities - Alice is **probably** in this office...calculated by ....

Maybe get into the concept that parts of HQDM will be sensitive themselves.

## Node identities

Need them - probably by preference at the physical layer.

We need to be able to refer to specific machines etc.

## Self-imposed constraints

Functionality requirement - I might have permission to read a document on a train, but as a user I may not be comfortable with that - I want to be able to add restrictions to myself.

## seL4 IOTA integration

Hand over token, activity happens, if it's an open-ended capability, hand it back to the user.

## Financial mechanism

Financial mechanism acts as a second, separate form of access control - have to have access as discussed here, but must also have a financial token to achieve something.  Digital security version of strength in depth.

