---
title: Humans and risk
parent: Security, risk, and trust
nav_order: 4
has_toc: false
---

# Humans and risk
{: .fs-9 .no_toc }


It's all socio - help the humans
{: .fs-6 .fw-300 }
----

The universe is a large and complex place, there are too many details to understand everything that is going on. 
Even if we could take an omnipotent view, understanding what actions to take to achieve desired outcomes, and all the actual implications of those actions is also impossible to fully predict.

As noted in our basic user needs.  Understandability, predictability and dynamic risk management.
Users are continuously trying to take actions that represent the best possible risk/reward trade-offs.
Hedge too much or too little - is to be inefficient/ineffective.
The closer user understanding, decision making, and subsequent actions aligns with some unknowable ideal, the more efficient and effective they will be.

Time and again studies show that we are innately terrible humans are with risk. 

Even though CONCRETE seeks to base itself of a small set of understandable principles (LINK), this will still generate a complex system of systems.
Holistic view - link to How complex systems fail.

CONCRETE foundations cannot 'solve risk' but it can recognise and support tooling and associated processes.

## Tools

User control but there's a lot of detail (eg could choose to pay to save some data on any node in the CONCRETE network).  There will be times when users will need this level of detail, but for much of the time, we can expect users to seek to defer to configurable automations (strategies, etc)

Example Replication factors for data/information.  I want my data to be replicated 3 times by default - I'd like a local to me copy and the rest just 'somewhere else'.  I'm going to give a presentation here - move my data there, so if the network goes down it's available - I'm happy that that counts as one of the replication points - so delete one elsewhere and save money.

This won't be one tool it will be many.  

These tools will need various sources of truth within the network, but also on the boundaries - What is an oracle?

The golden CONCRETE threads and payment system provide accurate useful information about where a user (or collectively and organisations) data, compute etc are.  This will help a lot with this kind of analysis.

(Contingency) planning.  Can't all fall back on the same thing.  Markets - and 4D planning tools (LINK)

## Human-centric interfaces

Different teams might be producing tools and feeds to help users make risk-related decisions, but these need to be developed with the human decision-maker in mind. The decision-maker needs a coherent holistic view that encompasses any and all such data/information.  This is not to suggest the need for a single standardised interface - this is not the case (all humans are different, all circumstances will be different), but it is to highlight the need for human-centric support.  Possibly the need for specialist service support users to set up their systems, and probably some best practices to enable those personnel (HQDM will help - see later).

As these human interfaces will need to be dynamically reconfigured, it will become important to have some common hmi design language, both for individuals and to maintain some group coherence.  This is a common finding in CONCRETE (LINK).  

## Services

In centralised systems we have things like network operation centres - this leads to users not understanding the actual risks that they're taking.  In Concrete this is inverted - users are in primary control. Yet, these services are still beneficial; these specialist personnel provide services that users can, and often will, elect to use.  Indeed, having a common standard foundation for larger numbers of users enables these services to become more effective and efficient (they are not talking in generalities).  Given the traceable nature of CONCRETE there is a great deal more opportunity to provide individualised support.

## Prior preparation and planning for the extremes

Zeroise and associated support for (re)building a CONCRETE network from scratch.  The trust modelling to understand how to do this - and hence to find the tools to enable it need to be completed.  The rest is best practice advice - that can also form part of the CONCRETE ecosystem.

Graceful degradation to complete loss.

HMI and processes that work when all the 'digital' is turned off.  

Example of Helicopter controls

This had to be designed into the system.

Technology paradox.

![Helicopter cockpit with lots of buttons](../../../../../images/current/helicopter_cockpit.png)

Re-write.

There are many buttons and controls in a helicopter cockpit.  However, only a few warrant being placed in the pilots' hands - on the flying controls themselves. Two of these found on many helicopters are the 'stabilization' and 'hydraulics' release switches.  The forces involved in manually controlling a helicopter are quite high.  Hydraulic assistance makes it easier for the pilot - power steering.  It is possible to control a helicopter without it - but it can be difficult and clumsy.  However, hydraulics systems are quite complicated and can go wrong - potentially locking the flying controls with hydraulic force.  Helicopters can also be a bit 'twitchy' requiring the pilot to constantly make simultaneous corrections to power, pitch, roll and yaw.  A stabilization system artificially (using the hydraulics) introduces control inputs to damp out the rate of pitch, roll and yaw.  This makes the helicopter slightly less responsive, but eases the workload.  Stabilization systems are complicated, and can sometimes go wrong - potentially adding high-speed uncommanded flying inputs. So-called 'higher flight modes' build further on this complexity and allow the pilot to select a speed, height, heading, or for the computers to follow a route.  If things are working correctly, the pilots might not even need to have their hands on the controls, they can be conducting other detailed, complex tasks.  However, when things go wrong, the helicopter can quickly start to fly in highly unpredicatble ways, the hierarchy of complexity makes these faults difficult to diagnose.  The stabilization and hyrdraulics releases allow the pilots to quickly remove complexity - quickly regaining control at the expense of having to concentrate on flying the aircraft.  The pilots can trade functionality to regain a simple state.  They do not need to have perfect knowledge of every aspect of these complex systems.  The pilots need a good working knowledge of their systems, but over the years this system design, including these switches, have been found to enable the complex behaviours of the system; they are a mechanism for suitably bounding complexity; so pilots can have their cake and eat it. 

{: .quote}
The same technology that simplifies life by providing more functions in each device also complicates life by making the device harder to learn, harder to use.  This is the paradox of technology and the challenge for the designer. \\ 
--- Don Norman, The Design of Everyday Things


## Chaos engineering and training

Cruel to be kind, or train hard fight easy.

Ethical stuff - some systems for some people need to be excluded (this is also useful information about where we need to support with things like redundancy)

Probably important that this happens from the start.

Test and evaluation.

Goes on already.

Not enough that we could react - we need to do the right thing on the night. Training, confidence.

In CONCRETE what this means is that there is a person/team who are going to impose failures.  This means that they need an authority that is higher than the users who are going to be subject to the failures themselves.  

Socio - we can also think about making human-side improvements:
Training - estimating risk - calibrating people's uncertainty estimates.

## HQDM

Need this to be clear

