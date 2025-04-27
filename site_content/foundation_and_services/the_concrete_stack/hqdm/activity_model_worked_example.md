---
title: Activity Model Basic Example
parent: HQDM
nav_order: 2
has_toc: false
---

![Activity Model Initial](../../../../../images/development_area/hqdm/CONCRETE_ActivityModelInitial.png)

![Activity Model Initial](../../../../../images/development_area/hqdm/CONCRETE_ActivityModelMid.png)

![Activity Model Initial](../../../../../images/development_area/hqdm/CONCRETE_ActivityModelFull.png)

```
<https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#0048a2aa-f1d2-444f-8817-3d25139e97b5> a hqdm:ordinary_physical_object;
    hqdm:beginning <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#7fd06ce6-ec2b-4375-b65a-559eb564ff69>;
    hqdm:ending diag:a3d04d4d-57c7-4ca3-814e-e3befcc333dc;
    hqdm:member_of_kind diag:dd944656-6b0b-45b3-8e8a-19bac21ae839, hqdm:ordinary_physical_object;
    hqdm:part_of_possible_world <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#0762f71b-7d19-4652-8546-4a47ce11a56f>.
<https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#0347bcb8-de0d-4e4d-83a8-69a1cb06d3ad> a hqdm:ordinary_physical_object;
    hqdm:beginning <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#7fd06ce6-ec2b-4375-b65a-559eb564ff69>;
    hqdm:ending diag:a3d04d4d-57c7-4ca3-814e-e3befcc333dc;
    hqdm:member_of_kind <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#9d9a1602-b5c9-4982-929b-193f2e8647d3>, hqdm:ordinary_physical_object;
    hqdm:part_of_possible_world <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#0762f71b-7d19-4652-8546-4a47ce11a56f>.
<https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#04057354-e5a7-4c68-9da5-2b60b69dd0c0> a hqdm:state_of_ordinary_physical_object;
    hqdm:beginning diag:ea91bbef-7846-4704-bef0-cbad63957271;
    hqdm:ending <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#64f73305-a0f7-4950-8c59-eb9d6b134ed4>;
    hqdm:member_of_kind hqdm:participant, hqdm:state_of_ordinary_physical_object;
    hqdm:part_of_possible_world <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#0762f71b-7d19-4652-8546-4a47ce11a56f>;
    hqdm:participant_in diag:aa4c6ea4-9b5e-4453-9a06-0af2967be184;
    hqdm:temporal_part_of <https://apollo-protocol.github.io/ns/2023/diagram-editor/diagram#62d01186-bdd9-4a1b-ac9c-1722866dc6fc>.
```

Although this worked example is simplified for brevity, it already indicates information management capabilities that are not currently available to the MOD and are in alignment with the MOD's recent Defence Drone Strategy, February 2024, Objective 3[^4].


------------------------------------

[^4]: [Defence Drone Strategy - The UK's Approach to Defence Uncrewed Systems](https://www.gov.uk/government/publications/defence-drone-strategy-the-uks-approach-to-defence-uncrewed-systems)