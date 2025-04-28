---
title: Matrix
parent: The CONCRETE stack
nav_order: 7
---
# [matrix] 
{: .fs-9 .no_toc }


Secure decentralised human communication
{: .fs-6 .fw-300 }
----

[![matrix logo](../../../../images/current/matrix.png)](https://matrix.org/)

Matrix is about secure decentralised human communication channels  

<span>Probable</span>{: .label .label-purple } While users will need matrix-style communications methods, and [matrix] was specifically designed with decentralised human communication in mind, this has yet to be analysed sufficiently in a CONCRETE context to claim that it is stable. This is not a reflection on [matrix] at all, just an observation about the maturity of CONCRETE.  

![matrix element communication channels such as chat and video conferencing](../../../../images/current/matrix_element.png)

Communication is clearly key to cooperation and teamwork. It has become increasingly common to find digital communication channels that are end-to-end encrypted for security. Although this end-to-end encryption can generate a secure communication pipe, these systems often use centralised servers to set up those connections.  The matrix protocol is a distributed, decentralised approach to secure communication. It has been used to enable many communication formats such as: text, community chat, VOIP, video conferencing, and virtual-reality meetings (without the need for a centralised potential point of failure).

While the applied cryptography techniques behind end-to-end encryption do secure the communication pipe itself, having CONCRETE end points based on trusted hardware and seL4 can be expected to add further security guarantees. 

Further sociotechnical analysis work is required (discussed further [here]({% link site_content/foundation_and_services/cutting_edge/communication_channels.md %})) to better understand how these kinds of communication channels might be incorporated into CONCRETE's information and security models.  Users might, for example, benefit from having identity-related support to help people to ensure that they are only communicating with the people that they want to (Bob really is the Bob that Alice wants to communicate with); or to aid users when they want link information within a meeting with the wider information whole.


 



