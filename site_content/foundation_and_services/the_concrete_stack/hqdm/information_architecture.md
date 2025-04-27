---
title: CONCRETE Information Architecture
parent: HQDM
nav_order: 1
has_toc: false
---

Exploring some of the key aspects of a system-wide CONCRETE Information Architecture.

## Trust Boundary

Building on the notion of an IA for CONCRETE [here](../../hqdm#concrete-information-architecture) one important consideration is that of how sufficient trust (confidence in the overall integrity, security, information protection inherrent in the system and its ability to do what's needed) can be achieved.  If the information being ['joined'](../../hqdm#information-architecture) in a systematic way to users and other information systems is sensitive to the organsations providing and using it across CONCRETE, the minimum protections need to be applied to secure it.  A basic consideration is how parties using CONCRETE can establish a confirmed connection with the CONCRETE _system_ itself.  

This should reasonably be done, to the level required, at the boundary of the IA.  Any user (or information system) that needs to connect to the IA must be able to meet a minumum number of connection requirements.  The requirements won't just be pre-arranged Identity and Access Management (IDAM), interface configuration and Information Assurance status validation checks, the system should be able to exchange chekable information records at every, and any particular, request to exchange information.

![Trust Boundary](../../../../../images/development_area/hqdm/CONCRETE_IATrustBoundary1.png)

While the diagram shows the Trust Boundary being at the edge of the IA that doesn't mean that every interaction between connected entities within CONCRETE is trusted.  Internal protections will be needed for specific exchanges between, and within, CONCRETE system components but they will be based on the agreed range of protections required (and known in advance) plus any variation signalled in any allowed CONCRETE information exchange interaction.  

The full set of trust mechanisms applied will be determined by the information context.  Crucially, the trust mechanisms are not expected to be based on pre-determined security labels applied to data 'packages' but will be computed by the CONCRETE [activity information](../../hqdm#activity-based-information-operations) exchanged during the exchange itself.  The green line indicating an exchange of information between Party A and Party B is therefore afforded a set of trust mechanisms and protections approriate that particular exchange and, in Information Assurance terms, holds for the entire span of the green line (not just the part within the CONCRETE IA).

{: .important }
There seems to be no precedent for an activity information-based exchange & information protection mechanism (that is computed at request time).  This is likely a novel part of CONCRETE that will need prototyping and detailed design, specification and validation.  However, the authors believe it to be necessary for the CONCRETE Vision and a way to break from the current, established methods that fall well short of what CONCRETE (and MOD) needs.

As each party will have their own Information System setting (perhaps including specific information security accreditations plus their own organisational information assurance policies and oversight) they will have the following conceptual setting with respect to CONCRETE.  This illustrates the importance of an IA that can be compatible with the CONCRETE system and the local information system(s) that it interfaces with.

![Trust Boundary Existing Systems](../../../../../images/development_area/hqdm/CONCRETE_IATrustBoundary2.png)

The figure below illustrates how the IA can conceptually support the transfer of CONCRETE-compliant information as long as the minimum exchange security requirments have been met.  In this case the Local Information Systems A & B have an integrated point of presence in the CONCRETE IA that allows Ͼ-compliant data to be held locally, trust to be established using local IDAM (with integrated records validating this within Ͼ) and connection requests to be established between Ͼ-connected Parties.  Consistency of information exchanges (requests and responses) can be achieved with one-or-many Master and Reference Data Libraries that are accessible to authorised parties within Ͼ. Although shown within the Ͼ-IA these will be Ͼ points of presence themselves, but will be accessible by those who have a confirmed need.

![Trust Boundary CONCRETE](../../../../../images/development_area/hqdm/CONCRETE_IATrustBoundary3.png)

{: .note}
Exchanges can be between Parties that are connected to the same Ͼ point of presence, individuals connected as in the diagram or with many parties (as contained in the activity-based Ͼ-information request).  There may be a number of types of Ͼ point of presence, the initial set will be determined during initial design.