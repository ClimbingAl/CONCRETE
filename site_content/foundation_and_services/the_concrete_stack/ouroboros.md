---
title: Ouroboros
parent: The CONCRETE stack
nav_order: 3
---
# Ouroboros
{: .fs-9 .no_toc }


Networking beyond TCP/IP
{: .fs-6 .fw-300 }
----

[![Ouroboros logo](../../../../images/current/ouroboros.png)](https://ouroboros.rocks/)

Ouroboros is about inter-process communication and networking.  The Ouroboros project is also under continued development and has a main site [here](https://ouroboros.rocks/).  Refer to the Ouroboros main site for detail, while this site will discuss the links to CONCRETE.

Most users have little, to no, knowledge about how data is routed around networks, but they do feel the effects of the underlying mechanisms. The dominant current approach TCP/IP (Transition Control Protocol/Internet Protocol) became the de-facto standard having been developed by DARPA, in association with US analogue telephone companies, to link approximately 11 computers in the internet's early predecessor, the ARPANET. Early TCP/IP design decisions haunt us to this day.  Current networking standards cause something of a security-related nightmare; they also needlessly limit networking capability.  Ouroboros can trace its roots back more than 40 years, but most recently as a specialisation of the [Recursive InterNet Architecture (RINA)](https://en.wikipedia.org/wiki/Recursive_Internetwork_Architecture)) approach developed by John Day[^pouzin].  Although this field has been subject to extensive academic research it is not as mature as, for example, seL4.  The need for something like Ouroboros is <span>Stable</span>{: .label .label-green } the maturity of the technology itself makes Ouroboros a <span>Probable</span>{: .label .label-purple} CONCRETE contender at this stage.  More positively, it is believed that many current Ouroboros gaps could be filled by other parts of the proposed CONCRETE stack.

[^pouzin]:
    Further academic links are collated by the [pouzin society](https://pouzinsociety.org/)

Although Ouroboros can be used to make arbitrarily complex networking capabilities, it achieves this by taking a dramatically simplified approach (when compared to TCP/IP). This is particularly useful for:

- **Security**. Current networking approaches open a vast potential attack surface to adversaries. Ouroboros substantially limits this, reducing the complexity of reasoning required to understand potential vulnerabilities.
- **Quality of Service**.  While it is impossible to guarantee a network-wide quality of service level (there are external factors beyond developers control), the Ouroboros model enables much greater opportunity to manage performance.
- **Multi-homing**.  Users currently expect devices to be linked to one network or another.  Multi-homing, the ability for a device to simultaneously reside on, and exploit, multiple networks, emerges easily from the Ouroboros approach. Resilience and redundancy are strongly enabled.
- **Mobile ad-hoc networks**.  Current networking technologies have to add specific support to better enable mobile nodes and their disrupted connections.  Again, the Ouroboros approach makes these kinds of in/out transient connections much easier to manage in the background.  Users would experience the effects of much greater resilience and redundancy despite natural and unnatural interruptions.  Much greater use could be made of the wider electromagnetic spectrum.

Some of the current open areas for development associated with Ouroboros might be solved by the rest of the CONCRETE stack. For example, Ouroboros is partially based on analysis about which entities in a network need to be named.  Within the CONCRETE approach, it is entirely reasonable to expect that trusted hardware would be individually named, and that individual processes (and their originating binaries) being run on seL4 would also have unique identifiers. This is very much in line with the needs of Ouroboros.  Further work is required to consider the potential amalgamation of Ouroboros and the seL4 approach to inter-process communication.  Putting this on a formal methods-style basis could be transformational for network security.

CONCRETE highlights the need for financial-style mechanisms to manage resource allocations including networking.  While Ouroboros already has various quality-of-service type mechanisms, further work would be required to experimentally amalgamate these with any financial-style mechanisms to better understand any performance and market implications.

Although Ouroboros is potentially a powerful alternative to current packet-switched networking techniques [^alongside], packet-switching is not the only means of transferring data from A to B.  Other techniques include physically moving storage devices, and other one-way communication techniques.

[^alongside]:
    Although many of the benefits are lost, Ouroboros can be run over or under existing TCP/IP networks making any transition much easier to manage.