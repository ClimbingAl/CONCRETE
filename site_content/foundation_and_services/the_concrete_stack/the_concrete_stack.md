---
title: The CONCRETE stack
parent: Foundation and Services
nav_order: 2
---

# The CONCRETE stack
{: .fs-9 .no_toc }


A technical sketch
{: .fs-6 .fw-300 }
----

The [basic user needs]({% link site_content/foundation_and_services/some_basic_needs.md %}) drive us to taking a distributed and decentralised approach, where to be foundational is to describe what it means to be a single abstract node.[^caveat]

[^caveat]:
    <span>To-do</span>{: .label .label-blue} This is a slight lie. The technical stack depicted assumes that all nodes have processors with operating systems.  While this is likely to represent many devices it would be possible to define a node in other ways - more work required.  Similarly, a raw processor is unlikely to be useful without other peripherals.  Further work is required to understand how these fit in with the trusted hardware layer. Amongst many other things, this signals the need for an approach to hardware identity.

![In a distributed decentralised system everything is just an abstract node](../../../../images/current/abstract_node.png)

The diagram below is a technical sketch of the make-up of an abstract node and some key ancillary functions. This should not be taken literally. The components shown act as a shorthand description; we should really add '-like' at the end of most of them. This is just a starting point for refinement.  The need for many of these components can be deduced directly from the basic user needs; some appear here out-of-the blue and are introduced later. From a major technical sub-component perspective though, **this is it**.  This section provides introductions to these components. The next socio-technical section only adds detail about how this would be configured and used.  

![stack of concrete components](../../../../images/current/CONCRETE_stack_w_bg.png)

| Component          | Description and links |
|:-------------------|:----------------------|
| Trusted hardware   | good swedish fish     |
| seL4               | good and plenty       |
| Ouroboros          | good `oreos`          |
| IPFS               | good `zoute` drop     |
| IOTA               | good swedish fish     |
| Wallet             | good and plenty       |
| [matrix]           | good `oreos`          |
| Security and Risk  | good `zoute` drop     |
| Time management    | good swedish fish     |
| Dongles            | good and plenty       |
| HQDM               | good `oreos`          |
| HMI Best practices | good `zoute` drop     |







