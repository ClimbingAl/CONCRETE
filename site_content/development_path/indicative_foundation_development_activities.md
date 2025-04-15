---
title: Indicative foundation development activities
parent: Development path
nav_order: 97
---

This is indicative only.

Mixed temporary teams of academics, coders, communicators, ontologists.



The development of a coherent set of standards and best practices can be likened to many other engineering challenges. A core team will develop and test individual components and bring these together to make working prototype systems.  Components can be developed and tested individually by different sub-teams.. These will be brought together in early prototypes that generate the understanding that paves the way for refined coherent solutions. The following list is indicative of the types of activity that could be expected as part of the Pg CONCRETE core development process.

Prototypes will often be tested in end-user communities. End-users, will be free to make use of these developmental systems should they wish.  The core team will aid decision makers in any associated early-adopter risk/reward analysis decisions.

<span>To-do</span>{: .label .label-blue} Subtle form of barrier we have separate pieces of software for things like CAD ..How do we beat Conway's Law? Tapping into computing processes for 'partial compute answers useful elsewhere' - effects on performance - monitoring, supervision, permanent 'debug mode' to monitor ...

1. TOC
{:toc}

## Digital resource management mechanisms

| Activity Number | 1                                                                                                 |
|:----------------|:--------------------------------------------------------------------------------------------------|
| Description     | To identify or develop the financial resource management mechanisms needed to maximise capability |
| Timing comments | One of the longest poles in the tent.  Start Early. This may become an ongoing task.              |
| Dependencies    |                                                |

Demand across a common network for digital-related resources such as storage, compute, and (contested) bandwidth, will always outstrip finite supply. Mechanisms to dynamically prioritise resource allocations are required. Financial market models (receiving and spending money/crypto-tokens; pricing, bidding, and gifting structures) are currently the only approach identified that could enable this. Technical infrastructure to enable these markets (eg IOTA-style contracts) need to be baked into the core.

There are many possible financial market models (How often do organisations receive 'money'? Are different tokens allocated for different resources? How are prices determined?).  The most challenging part of this task is the experimentation required to determine which mechansisms maximise organisational capabilies. These experiments require the live/virtual HMI development environments (below) to conduct development and test activities with real-world personnel. 

Expect the need for personnel with game industry skills, and human-factors researchers, to help to create tools, and associated instrumented environments to conduct developmental testing (for this and many other activities)

## Information security model

| Activity Number | 2                                                                             |
|:----------------|:------------------------------------------------------------------------------|
| Description     | Multi-level security.  Development of the user-managed need-to-know approach. |
| Timing comments | Start early - users could be expected to find early benefits.                 |
| Dependencies    | Nil.                                                                          |

The CONCRETE socio-technical approach to multi-level information security allows users to manage need-to-know access to any piece of information.  It also allows users to manage administrative rights such as lists of personnel who can modify the need-to-know access list etc.  This approach also enables a powerful approach to collaborative working.

There are many potential security-related edge-cases to consider.  The socio-technical approach needs to be developed and tested with end-users. Experimental development will provide groups of users with early versions of these tools. Early mock-ups may use simpler centralised approaches for experimental purposes.  Distributed and decentralised versions would be developed as part of the main foundation.


## Boss-Based Access Control

| Activity Number | 3                                                                                   |
|:----------------|:------------------------------------------------------------------------------------|
| Description     | Developing a socio-technical approach to raw data access control.                   |
| Timing comments | A central part of the CONCRETE approach.  De-risk and exploit as early as possible. |
| Dependencies    | Data obfuscation / synthesis tools (Activity 13).                                   |

Boss-Based Access Control (BBAC) is a proposed socio-technical approach to the management of access to raw data. Early experiments can use mock-ups to test the socio- aspects of this approach including early development of the associated data caputre and monitoring tools that will be needed by organisational guards (similar to current fraud detection techniques used by banks) and more generally by the user community.

## Layered security tooling

| Activity Number | 4                                                                                                                               |
|:----------------|:--------------------------------------------------------------------------------------------------------------------------------|
| Description     | Developing the wider approach to layered physical security.                                                                   |
| Timing comments | Relatively few dependencies hence a parallel workstrand                                                                         |
| Dependencies    | Related activities - Cryptographic core + Trusted physical compute (Activity 17) - Full stack physical prototypes (Activity 20) |

Many elements of the core CONCRETE approach (eg BBAC and information security) will use cryptographic keys (long strings of numbers) to identify personnel and secure data and information.  CONCRETE also requires and enables new physical security mechanisms. There are many aspects to physical security. CONCRETE's decentralised/distributed theme aligns closely with the concept of security in depth.  Many systems and measures can be expected to be developed and managed independently (assuming that each could be compromised) while collectively contributing to the security whole.

This thread will develop a coherent set of cyber-physical standards and best practices (dongles/readers/2FA, tracking, biometrics, IDAM, digital locks, entry gates etc, and their links with the CONCRETE stack). Testing can be exepected to include penetration testing of mock working environments. 

## Chaos engineering and live cyber-risk awareness

| Activity Number | 5                                                                                                                                                       |
|:----------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------|
| Description     | Tools and best practices to enable personnel to make great cyber-related risk/reward decisions.                                                     |
| Timing comments | Technical support for chaos engineering needs to be including in early prototypes.  Cyber-risk awareness requires some knowledge of CONCRETE end-state. |
| Dependencies    | Nil.                                                                                                                                                    |

Boss-Based Access Control, user-managed information security, and the financial model for digital resource management all involve users making dynamic risk/reward decisions.  These are necessary to enable the personnel to flexibly adapt to changing circumstances.  Users should understand the rewards associated with their work, this activity will help to ensure that they have the best tools and processes available to help them to understand and react to changing cyber-related risks.

Cyber-related risks are not voodoo; they are quantifiable. Some risks, such as the potential for data loss from a hard-drive failure, are relatively static.  Others such as threats from hostile actors are dynamic - requiring up-to-date assessments of capability and intent. This activity will develop tooling to enable users and organisations to understand risks, plan responses, and potentially provide automatically reactions to changing threat pictures. 

As part of this, a chaos engineering approach will be adopted. This will enable (technically supported) organisational user-leaders to purposefully inject real faults/events into their own system. Personnel and organisations will be permanently dealing with cyber events as part of their everyday digital lives (the cyber version of: train hard, fight easy).  The technical machinery to enable this needs to be built into the core capability.

## Data-related algorithms

| Activity Number | 6                                                                     |
|:----------------|:----------------------------------------------------------------------|
| Description     | Developing / choosing data-related algorithms to maximise capability. |
| Timing comments | One of the earliest algorithmic components required in CONCRETE.      |
| Dependencies    | Nil.                                                                  |

Distributed and decentralised systems need specific mechanisms to enable users to work with data: storage/recovery, universal naming, search, discovery, updates etc. These data-related algorithms will be a core part of the foundation.  Hence, preliminary development of this functionality can be expected to be one of the first technical activities to enable wider developmental progress.

End-users are not expected to work directly with these algorithms, but they will feel the effects of them (latency of systems, core system bandwidth overheads etc). Representative environments will be needed for testing and development.  This work will eventually be tested in live/virtual environments. This is likely to become and ongoing task requiring continued research and development. 

## High Quality Data Model (HQDM)

| Activity Number | 7                                                         |
|:----------------|:----------------------------------------------------------|
| Description     | Developing the tools and experience associated with HQDM. |
| Timing comments | No dependencies.                                          |
| Dependencies    | Related - Programming techniques for a CONCRETE World.    |

HQDM is an ontological standard that enables the meaning of any and all data to be accurately and consistently described.  The foundation will require all data to be described using this approach.  This is key to digital capability; it enables digital-related velocity, flexibility, efficiency, and interoperability.  Associated tools, processes, and experience need to be developed.  HQDM is not currently in common use in the wider software industry.  This activity should also seek to rapidly accelerate initiatives to generate how-to guides and other training material to help to on-board developers who are new to this field.


## First-class links and information quality

| Activity Number | 8                                                                    |
|:----------------|:---------------------------------------------------------------------|
| Description     | Development of data-object links and associated tooling.             |
| Timing comments | Few technical dependencies, early experimentation possible.          |
| Dependencies    | Data-related structures and algorithms.  Information security model. |

Current hyperlinks are simple one-way references embedded within documents.  CONCRETE analysis highlighted the need for more powerful links that are stand-alone objects - Wendy-links.  These are needed, for example, to be able to map, understand, and maintain data about relationships between sources of information.  These links need to be developed in ways that respect the security mechanisms associated with CONCRETE. Users will need tooling to exploit these links to their full potential.  

## Decentralised communication tools

| Activity Number | 9                                                                    |
|:----------------|:---------------------------------------------------------------------|
| Description     | Embed decentralised communication tools into the core foundation.    |
| Timing comments | Few technical dependencies.                                          |
| Dependencies    | Data-related structures and algorithms.  Information security model. |

Users will need best-of-class secure communication tools that work in decentralised environments.  Standards such as Matrix (messaging, chat rooms, video conferencing, VR) already exist.  These may need to be modified or used in ways that enable organisational guards.  This activity will embed this functionality withing the core set of standards.  

## Trust boundary management and tooling

| Activity Number | 10                                           |
|:----------------|:---------------------------------------------|
| Description     | Gateways, tooling, and associated processes. |
| Timing comments | Few technical dependencies.                  |
| Dependencies    | Information security model.                  |

A CONCRETE-based shared-data environment might span multiple government departments eg the MOD and the UK security services. The wider the scope, the more capable a system can be. However, there will always be a limit or boundary between those who are within the system and those that are not (driven by factors such as trust, shared values, and legal constructs).  There will always be a need to share data, information, and other capabilities across these boundaries (Gov, Industry, International etc).  This may be to other CONCRETE-based enclaves, or to entirely different systems.  This activity will develop the tooling, techniques, and associated governance frameworks to enable this gateway functionality.  

## Trust management tooling

| Activity Number | 11                                                  |
|:----------------|:----------------------------------------------------|
| Description     | Tools and interfaces to manage trust between nodes. |
| Timing comments | Few technical dependencies.                         |
| Dependencies    | Information security model.                         |

Decentralised and distributed CONCRETE nodes need mechanisms to enable them to join a network from a factory-reset state. Some functions, such as chaos-engineering, require permissions and authorities to be transferred from an originating node to others.  This functionality needs to be built into the core system. In extreme situations, pepple may need to reset/detach from a potentially compromised system and restart this process from scratch.  The human machine interfaces associated with node management need to developed with users (not just the IT crowd) in mind.  

## Spacetime synchronisation mechanisms

| Activity Number | 12                                                                                                                                   |
|:----------------|:-------------------------------------------------------------------------------------------------------------------------------------|
| Description     | Develop standards, methodologies, interfaces, and strategic equipment to enable spacetime synchronisation. |
| Timing comments | Nil.                                               |
| Dependencies    | Related: HMI, HQDM development.                                                                                                      |

Clocks play a key role in digital capabilities.  Users and organisations can expect to gain many competitive advantages from increased clock accuracy and improved node-to-node synchronisation.  As clock accuracy improves, and as more space-based systems are incorporated into systems-of-systems, relativistic spacetime effects become ever-more important to take into account.  

A robust, resilient approach to spacetime synchronisation across is required. As spacetime synchronisation affects user and organisational risks and capbilities; its management is expected to become an operational function requiring dedicated tooling. This activity will develop synchronisation standards, methodologies, and interfaces.

The need for spacetime-related standards extends beyond clocks and time.  HQDM (Activity 7) is a 4-dimensional ontological approach; the MOD needs to adopt a consistent approach to describing concepts such as positions, components and sub-components etc.

## Data obfuscation and syntheteic data tools

| Activity Number | 13                                                                                 |
|:----------------|:-----------------------------------------------------------------------------------|
| Description     | Develop a library of algorithms for data obfuscation and sythetic data production. |
| Timing comments | Start early to anticipate many user needs.                                         |
| Dependencies    | Enables BBAC approach.                                                             |

Boss-Based Access Control  requries users to select data sets with the least possible information content commensurate with their task.  Users need algorithms that can reliably strip or obfuscate otherwise sensitive data.  It also needs algorithms to enable personnel to produce statistically relevant sythetic data sets.  This activity will start to develop a library of these Government-assured algorithms. 

## Statistics, uncertainty, and probability

| Activity Number | 14                                                                                             |
|:----------------|:-----------------------------------------------------------------------------------------------|
| Description     | Develop standards and best practices associated with statistics, uncertainty, and probability. |
| Timing comments | Nil.                                                                                           |
| Dependencies    | Related: HMI development.                                                                      |

Statistics, uncertainty, and probability can be expected to become increasingly important as all aspects of society become more data-centric. Statistics, uncertainty, and probability are likely to become everyday operational tools. Unfortunately, studies repeatedly show how poor human intuition is with these concepts; standards and best practices are required.  This might include the development of standard visualisations, approaches, and algorithms.  It might also identify the need for specialist support personnel or standard training packages.

## Networking

| Activity Number | 15                                                       |
|:----------------|:---------------------------------------------------------|
| Description     | Developing communication and networks-related standards. |
| Timing comments |                                                          |
| Dependencies    | Related: HMI development. Financial models.              |

There are various communications and networking-related standards, best practices, and tools to develop and bring into the foundation. Much of this work will be informed by the HMI and resource management research activities. The outcomes of this may lead, for example, to the need for new networking standards and firmware developments for routers. Beyond the user-facing aspects of networking and communication, other standards such as hardware and associated test methodologies will be developed.

## Applied category theory

| Activity Number | 16                                                                                        |
|:----------------|:------------------------------------------------------------------------------------------|
| Description     | Learning to use the foundations of computer science to generate world-class capabilities. |
| Timing comments | Long lead times - get started.                                                            |
| Dependencies    | Related: HQDM, HMI (broad user needs analysis)                                            |

Although not immediately apparent, the computer games industry is a common driver of cutting-edge digital developments (hardware and software).  The desire for richer, immersive, often multi-player experiences leads to developments in many foundational areas such as networking techniques, efficient computing resource usage, and high-speed physics simulations.  These technical advances are often being made by tiny numbers of enthusiasts, academics, or industry engineers. These developments are rarely directly exploited in individual games; instead, these personnel often make tools for higher-level engineers, who in turn may be making tools for games artists (who need little technical knowledge).  This layered approach is common. We can expect to adopt a similar pattern.  World-class user-facing digital capabilities that can be adapted rapidly to meet changing needs require these well understood, powerful libraries of common tools.

The deep foundations of computing lie in the intersection of applied physics and mathematics (physics-related developments are covered later).  The mathematical foundations are loosely referred to here as applied category theory (early protagonists in this area include Ada Lovelace and Alan Turing). As with many foundational science and technology areas eg theoretical physics,  developments in this field may not be directly understood by end-users, but their application can bring profound benefits. Part of the core long-term mission is to learn to how to better engage with this community, and reap the rewards.  This thread will seek to establish lasting and efficient engagement mechanisms between users and foundational computing communities.  

There are a number of areas for potential early development. As an example, we could expect analysis of user activities to highlight that large numbers of personnel and organisations are involved in 'planning' (over many different fields, scales, and timescaless) and 'execution'. A better understanding of the fundamental structure of the acts of planning and execution could lead to new best practices for how to strucutre associated software tools. Common high-level themes of the benefits of category theory-based developments include improvements in software coherence, interoperability, composability (eg support for plans within plans), and efficiency.  From a user perspective, planning and execution process could become substantially more coherent across many currently disparate fields.  This could be expected to make organisations and users more efficient, and effective.

## Trusted hardware and seL4

| Activity Number | 17                                                                   |
|:----------------|:---------------------------------------------------------------------|
| Description     | Hardware and operating system-related standards and best practices.  |
| Timing comments | Start early. An ongoing research task with an exploitation drumbeat. |
| Dependencies    | Related: HMI (broad user needs analysis)                             |

Various standards and best practices associated with computing hardware and the associated operating system are required.  When compute workloads are decentralised and distributed, there is a greater need for highest-common-denominator standards in areas such as security (trusted compute) and even mathematics (we don't want the answers to fire-the-missile maths calculations to differ depending on where, and when, they are computed).

The implications of real-world use-case environments and computational workloads need to be understood and monitored over time for hardware optimisation (ASICs, FPGAs, GPUs, photonics, quantum computing etc). Various CONCRETE approaches may themselves be best served in hardware, not software. 

## Data storage technologies

| Activity Number | 18                                   |
|:----------------|:-------------------------------------|
| Description     | Long-term data storage technologies. |
| Timing comments |                                      |
| Dependencies    |                                      |

There are many benefits to be gained from live data networks, but there are also many benefits to be gained from mining large-scale long-term data stores.  Given its potential value, governments  and organisations can be expected to need to store vast amounts of data.  Even with modern fibre networks, it is often quicker, and substantially cheaper, to physically move data storage media around the globe. There are many different technical approaches to data storage and many different considerations. 

## Programming techniques for a CONCRETE world

| Activity Number | 19                                |
|:----------------|:----------------------------------|
| Description     | Programming best practices.       |
| Timing comments |                                   |
| Dependencies    | Related: Applied category theory. |

Developing high-quality software for use in a decentralised, distributed system can be expected to be non-trivial. Substantial benefit can be expected to be gained by developing and communicating standards and best practices associated with software development in a 'CONCRETE world'. 

## Full-stack physical prototyping

| Activity Number | 20                                       |
|:----------------|:-----------------------------------------|
| Description     | Developing full-stack prototype systems. |
| Timing comments |                                          |
| Dependencies    | Related: All.                            |

In order to develop standards and best practices, full-stack prototypes of various different form factors (large 19in rack mount hardware, laptops, to miniaturised systems) will need to be made and tested (individually and collectively).  

## Red team

| Activity Number | 21                                                              |
|:----------------|:----------------------------------------------------------------|
| Description     | A dedicated team searching for errors or potential improvements |
| Timing comments |                                                                 |
| Dependencies    | Related: All.                                                   |

To mitigate against groupthink and other biases, this is a purposefully arms-length team with access-all-area passes.  This team would conduct their own research and development activities to enable them to challenge the status quo.  This team needs sufficient funding to keep up with the pace of core development activities.

## Internal and external communication

| Activity Number | 22                                                                      |
|:----------------|:------------------------------------------------------------------------|
| Description     | A dedicated team (or teams) aiding internal and external communication. |
| Timing comments |                                                                         |
| Dependencies    | Related: All.                                                           |

There will a huge need for both internal and external communication and documentation-type activities, especially when developmental velocity is key. The deep technical specialists need to be supplemented and supported by groups with a variety of complementary skills: graphic design, content creation, videography etc. 

## Formal methods tooling

| Activity Number | 23                                                                     |
|:----------------|:-----------------------------------------------------------------------|
| Description     | A dedicated workstrand developing tools associated with formal methods |
| Timing comments |                                                                        |
| Dependencies    | Related: Foundational stack and all dependable tools.                  |

Much of the strength of the CONCRETE foundation comes from its correctness and dependability.  This dependability is generated by an approach known as 'formal methods'.  This involves proving (in the mathematical sense) certain properties about designs. This is quite hard; it also needs to become more common.  This activity would develop tools to better enable engineers to utilise formal methods in their day-to-day activities.

