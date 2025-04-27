---
title: HQDM
parent: The CONCRETE stack
nav_order: 11
has_toc: false
---

An information-based operational system that ensures users get what they requst[^1] in accordance with their need, context and roles should have a system-wide Information Architecture (IA).  Without an established IA, with particular properties that enable it to service all the agreed initial and future information requirements, the CONCRETE system will be limited in capability (scope) and will be constrained to facilitating data transfers only, where the system is not 'aware' of the information in those data transfers.  There are plenty of data transfer systems available today; what they lack is the system-level information that allows them to be part of the decision support functions.

This page sets out:
- What an IA is
- What characteristics and compnents it must have to be fit for the CONCRETE Vision
- How it could be implemented

## Information Architecture

The term has been used in various ways since the early 1980s.  For the advanced nature of CONCRETE we shall state that IA refers to the system-wide design, and related committments, that allows the linking of information that is fit for decision support to those (other information systems and, crucially, decision makers) that need it.  'Linking' implies the request for, finding and subsequent provision of the information in a form that is fit for the agreed purpose.  Essential considerations for a suitable IA are the data/information model choices, the means by which these choices can be joined together (or integrated) across the extents of the CONCRETE system and its users, and the ongoing methods that allow it to keep pace with changing user needs (individually and in aggregate).  It is the **integrated** nature of the information operations and the need to add to them without re-engineering CONCRETE that make this use of the term Information Architecture markedly different from previous uses.  The IA necessarily has to support the operational and management processes that rely on it including the roles and authorisations that are needed for each instance of each process (initially identified and future ones).  Any designed system components, interactions and automated processes must be compatible with the IA (not the other way round).  A key reference for the IA and the related information system components is [^2], Chapter 4 and the Part 3, Chapters 10-16,

## CONCRETE Information Architecture

A few general points about the CONCRETE IA[^3]:

**Ͼ-IA1** The CONCRETE IA extends beyond the transport, I/O and internal storage parts of CONCRETE.  This means that other systems interfacing with CONCRETE must be minimally compliant with the CONCRETE IA to allow the information interactions that their users need.

**Ͼ-IA2** Within the CONCRETE IA information operations are managed according to the system-wide IA.  Any information (data) passed that is not based on the CONCRETE IA MUST be wrapped in a CONCRETE IA context.  Only CONCRETE IA contexts are stored and processed within the CONCRETE IA.

**Ͼ-IA3** The CONCRETE IA must have a single information model that has the following properties: 

- [x] It must be universally consistent, for all inital and future CONCRETE applications.
- [x] It must therefore be formally extensible (to satisfy current and future information requirements).
- [x] It must be shareable and accessible within CONCRETE and the connected (compliant) information systems.


![infoarch](../../../../images/development_area/hqdm/CONCRETE_InformationArchitecture1.png)

An expansion of the CONCRETE IA is [here]({% link site_content/foundation_and_services/the_concrete_stack/hqdm/information_architecture.md %}).  Parties A-D are used to illustrate scenarios that CONCRETE should be able to handle (e.g. to allow Parties A to request information from Party B &/or C without Party D being privvy to the request).  The CONCRETE IA is necessarily wider in scope than any input/output (I/O) system that supports the CONCRETE Information Operations.  Parties don't just need to be persons.  Other information systems, including mobile platforms and computer-controlled assets, can be conceptually connected using CONCRETE.


## CONCRETE Information Model
The essential part of the CONCRETE IA is an integration data model.  An integration data model is one that can be used universally as the root of data models for all information operations within the IA in which it is used.  Its role is central to the IA and must be the only data model used to service the information operations within the Ͼ-IA.  The theoretical underpinnings of an integration data model are grounded in formal logic, metaphysics (a field of ontology) and related fields.  A survey[^4] of the available models that justifies the selection of HQDM, and the other candidate models, is publicly available.  A summary of key requirements of an integration data model for Ͼ-IA are:

**Ͼ-IM1** The information model must have a fixed (stable) root structure to underpin all initial and future CONCRETE information requirements.

**Ͼ-IM2** It must be based on ontological comittments that allow the universally consistent representation of anything that is actually or possibly 'real'[^5].

**Ͼ-IM3** Information managemeng processes, implementation technologies and tooling must be available to ensure that the Ͼ-IM can be used for the identified requirements (individually and in aggregate).


{: .highlight}
HQDM is the name given to the proposed CONCRETE Integration Data Model.  Whether HQDM is sufficiently close to being "good enough" for this role in Ͼ is yet to be determined but it seems closest to meeting the requirements below.  Other candidates are BORO-based models such as [ISO-15926-2](https://www.iso.org/standard/29557.html) (the rest of this standard is relevant to the Ͼ-IA) and [IES](https://www.informationexchangestandard.org/ontology/ies) (currently undergoing a major update that may have the structural integrity to support the Ͼ requirements).

{: .important}
There is no precedent for adopting and using an integration data model like this.  However, without it there is no computable mechanism to meet the CONCRETE requirements.  By definition, without a suitable integration data model CONCRETE will not be integrated.

## Activity Based Information Operations
The only role for information that is managed in an organisational setting is decision support. Decisions that are identifiable in advance are typically part of an organised *activity* based on an agreed process.  Current information systems in large organisations tend to be very limited in their scope because the business process(s) that they support were defined prior to the implementation of those systems.  Their information architecture, data model(s) and the transactions they allow are fixed around these processes.  For CONCRETE to meet its Vision, it needs to avoid this legacy approach to implementing data-based information systems[^6].  

The proposed way of doing this is to harness the expressive power of the Ͼ-IM and allow processes (that we'll call Activity Models) to be dynamically specified, represented in Ͼ and agreed in a consistent manner.  Anything that happens in the real world is Activity and those things involved in any particular Activity are identifiable participants.  An Activity that can be identified in advance can be modelled using HQDM.  Such an Activity Model is a collection of the reqired classes and the rules around the participants (e.g. what is allowed, pre-conditions, what the kind of expected participants are, etc forming the information management requirements for any actual instance of the activity).  There is a published methodology for identifying the information requirements[^7].  All of the transactions that happen across/within the Ͼ-IA are mediated by HQDM-based Activity Model patterns that are dynamically added (and removed) and are accessible by those who need them.  Activity Models will be needed to support the generation of these new Activity Models, with the key point being that they are developed within the Ͼ-IA and are consistent with the Ͼ policies, security and performance framework.  

{: .important}
Notably, it is the Activity Models themselves that set the information integration architecture ("the interfaces between systems and the data models of the interfaces"[^2] )

### An illustration of activity modelling
Everything that the military does is activity.  The eccompasses a vast range of kinds of activity, with the objective of the Ͼ Vision to support, in the limit, any and all of them.  To illustrate the sorts of information-based activities that could be part of this large array, here are some examples of requests for:

1. A record of UAV observations over Territory X in the build up to the last attack by the enemy (or in the last 24hrs, or to be provided hourly including tracks during that period).
2. Information on the known Unmanned Ground Vehicles used by an adversary including original language, translations and images to support an analyst triaging material obtained about them in a time-pressured setting.
3. The capabilities and status of 10 Foxhound Protected Mobility Vehicles due to arrive for deployment at Airfield Y tomorrow to confirm that they have capacity for some extra equipment.
4. A list of personnel who were deployed to Area Z in the last 9 months and their current contact information.
5. The requirements for and maintenance procedures of a particular Embraer Phenom T.1 training aircraft that is to be based temporarily at airfield W.

Ok, so some of these are going to be more complex than summarised above, but they are all plausible activities that a large orgainsation like the MOD would expect to be able to support.  In fact, they are compatible with the aspirations laid out in the UK Data Strategy for Defence, Edition 1 (and summairsed similarly in its Foreword)[^8].  Complex activities can be broken down into constituent parts that are less complex.

<details markdown="block">
<summary>How to agree new Activity Models</summary>

The following features are necessary to develop new Activity Models.

- [x] A process for developing them is needed (this is also an Activity Model), with documentation, tools, training, management and governance measures.
- [x] Those who have the domian knowledge relevant to the activities in question must be involved and be part of the agreeing that the resulting models are likely to be fit for the intended purpose.
- [x] They must be validated with one or more actual instance of the activities being modelled.
- [x] They should be reviewed and updated within a minimum period set by those involved.

</details>

### Activity Scenario

![Activity Model Initial](../../../../../images/development_area/hqdm/CONCRETE_ActivityModelInitial.png)

Finally, an additional benefit for the oversight and improvement of defence activities is that there is a formal record of the instances of each activity involved in an information exchange using CONCRETE.  This will significantly improve the information available to analyse and improve upon the activities.

## Comments on the proposed Ͼ-IA approach

TBC
... and related records management.  Ensures the full (or at least a minimally complete set of) information is present within CONCRETE.

... can, and should, include the speculative request for information to multiple parties (e.g. all those that have subscribed, perhaps automatically, to published activity models)

... including IDAM, BBAC, Computable sensitivity classification, 

... c.f. Zero Trust now and the Ͼ-ZAIT Zero Assumed Information Trust




---------------

[^1]: An assumption for the moment is that there will always be a request that initiates a, or a sequance of, exchanges.  This may also include group-/system-wide broadcast messages.

[^2]: [Developing High Quality Data Models](https://doi.org/10.1016/C2009-0-30508-5), Dr Matthew West, 2011 with an informal introduction to it [here](https://github.com/gchq/MagmaCore/wiki).

[^3]: These points are numbered for reference as necessary properties of the CONCRETE design (Ͼ==CONCRETE).

[^4]: [A Survey of Top-Level Ontologies](https://www.cdbb.cam.ac.uk/files/a_survey_of_top-level_ontologies_lowres.pdf).

[^5]: This is a brutal requirement.  A basic introduction to the model is [here](https://climbingal.github.io/HqdmPatterns/introducing_hqdm/basic_intro_to_hqdm/).

[^6]: Attempts to avoid structured approaches to information operations do not address the underlying information management concerns that CONCRETE has to address.  

[^7]: The [Information Requirements Methodology](https://github.com/Apollo-Protocol/information-requirement-methodology/blob/main/information-requirement-methodology.md) and an introductory document [An Integrated Approach to Information Management](https://www.cdbb.cam.ac.uk/files/process_model.pdf).

[^8]: [Data Strategy for Defence, Edition 1](https://assets.publishing.service.gov.uk/media/614deb7a8fa8f561075cae0b/Data_Strategy_for_Defence.pdf)