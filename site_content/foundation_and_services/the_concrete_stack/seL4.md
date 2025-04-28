---
title: seL4
parent: The CONCRETE stack
nav_order: 2
---
# The seL4 Microkernel
{: .fs-9 .no_toc }


Security is no excuse for bad performance
{: .fs-6 .fw-300 }
----

[![seL4 logo](../../../../images/current/seL4.png)](https://sel4.systems/)

Most users will be aware of operating systems such as Windows, Android, iOS, and Linux.  This is the lowest-level system software that manages all underlying hardware and other software resources . seL4 (ess-e-L-four) lives in this same operating system software family, and has some particularly useful properties. This open source project, with strong government and academic roots, has been in development for some decades and has its own website [here](https://sel4.systems/).  seL4 is in continuous development, please look to that website for any detail, we concentrate here on why this is important from a CONCRETE perspective.

seL4 has been developed as a performant trustworthy operating system (actually a miniature operating system called a 'microkernel'). Unlike most other operating systems, the trustworthiness of seL4 is not a function of 'hope', 'good engineering practice', and 'experience', but is based on a series of highly-formal mathematical proofs. seL4 controls everything about its underlying hardware, and any software that is based on it.  Without this component, and its proofs, CONCRETE could never generate a solid foundation, there would always be a possibility that bug could lead to a critical vulnerability.

![stack of concrete components](../../../../images/current/CONCRETE_stack.png)

Security is incredibly important within CONCRETE, particularly as multiple users (including potential rogue actors) could be using the same hardware. seL4 provides a mathematically guaranteed separation between processes. A hostile actor who has access to a node cannot affect or monitor somebody else's process.

One of the core, proven, features of the seL4 microkernel is its '[capability-based access control model](https://sel4.systems/About/seL4-whitepaper.pdf)'[^capability]. A capability is a unique unforgeable token that bestows on its possessor specific permission to access or use one or more resources within the system itself (very fine-grained access to sub-components, processes, networking, specific areas of memory, disks etc).  Importantly, without a capability token, nothing happens. The CONCRETE approach to access control is based on this.  These unforgeable capability tokens would be used throughout a CONCRETE network to bestow revocable capabilities on users (whom themselves are identified by unforgeable cryptographic tokens).  This enables a mathematical golden thread of control from authorisers to hardware. 

Software developed for the seL4 operating system can choose whether to continue with the formal proof methodology (or not).  Software developed in this way (often called 'formal methods') can take longer to produce, but it generates software with proven qualities associated with dependability, security, performance etc.  The expertise and associated tooling to enable this kind of development have been growing over recent years. This can be expected to become a key differentiator for quality software development in the future. The rest of the CONCRETE stack 'above' seL4 can be expected to be developed using these techniques.

[^capability]:
    The capability-based access control mechanism adopted by seL4 is the most powerful known approach to security in operating system design.  Most other operating systems are based on a simpler 'access control list' approach that has known vulnerabilities (see: [the confused deputy problem](https://en.wikipedia.org/wiki/Confused_deputy_problem); or for a longer-form technical essay see: [here](http://habitatchronicles.com/2017/05/what-are-capabilities/)) 

Operating systems can be huge pieces of software.  seL4, as the 'microkernel' software class name suggests, is tiny in comparison; this is double-edged.  Large operating systems need significant resources to run; they are not well suited to small, low-power, internet-of-things devices.  seL4 is not constrained in this way.  However, the additional software associated with non-trustworthy operating systems means that they can often be used out-of-the-box with many regular pieces of generic off-the-shelf hardware; seL4 developments will require more bespoke software to be produced for any particular node design, although this may, in turn, drive more trustworthy hardware design features.


<span>Stable</span>{: .label .label-green } seL4 itself is considered stable within CONCRETE.  However, it is also under constant development.  There are many areas where these developments would be useful eg development associated with timing channels (preventing the need for particular security work-arounds), and better formal linking between seL4 and hardware (particularly for multi-core-style architecture use).  CONCRETE also highlights the potential for improvements associated with aligning the concepts of on-chip inter-process communication and wider networking (eg Ouroboros). 


