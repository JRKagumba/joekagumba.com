---
title: "Movement Modelling"
date: 2020-06-08T08:06:25+06:00
description: Sample post with multiple images, embedded video ect.
menu:
  sidebar:
    name: Movement Modelling
    identifier: AA-02
    parent: Academic Articles
    weight: 102
hero: modeling_movement.png
tags: ["Markdown","Content Organization","Multi-lingual"]
categories: ["Basic"]
---

The following is an informal explanation of my thesis study. For a more formal reading, [here](https://www.proquest.com/openview/0aa707187ddd21fcf5a9ea1b847cb278/1.pdf?pq-origsite=gscholar&cbl=18750&diss=y) is a link to the published version. This written piece will cover what the study was about, the study design, why it may be important and future research directions. 

---


{{< mermaid align="left" >}}
graph LR;
    A([Participant]) -->|Tool Type| B[[Bosch]]
    A([Participant]) -->|Tool Type| C[[Cleco]]
    B -->|Joint Type| D[Hard]
    B -->|Joint Type| E(Soft)
    D -->|Target Torque| F{30 Nm}
    D -->|Target Torque| G{55 Nm}
    D -->|Target Torque| H{75 Nm}
    E -->|Target Torque| I{30 Nm}
    E -->|Target Torque| J{55 Nm}
    E -->|Target Torque| K{75 Nm}
    C -->|Joint Type| L[Hard]
    C -->|Joint Type| M(Soft)
    L -->|Target Torque| N{30 Nm}
    L -->|Target Torque| O{55 Nm}
    L -->|Target Torque| P{75 Nm}
    M -->|Target Torque| Q{30 Nm}
    M -->|Target Torque| R{55 Nm}
    M -->|Target Torque| S{75 Nm}

    style A fill:#808080,stroke:#333,stroke-width:4px

<!-- Bosch vs Cleco -->
    style B fill:#005aff,stroke:#333,stroke-width:2px
    style C fill:#ffa500,stroke:#333,stroke-width:2px

<!-- Hard vs Soft -->
    style D fill:#00b41a,stroke:#333,stroke-width:2px
    style E fill:#b4009a,stroke:#333,stroke-width:2px
    style L fill:#00b41a,stroke:#333,stroke-width:2px
    style M fill:#b4009a,stroke:#333,stroke-width:2px

<!-- 30Nm, 55Nm, 75Nm -->
    style F fill:#ff664d,stroke:#333,stroke-width:2px
    style G fill:#ff2500,stroke:#333,stroke-width:2px
    style H fill:#b41a00,stroke:#333,stroke-width:2px
    style I fill:#ff664d,stroke:#333,stroke-width:2px
    style J fill:#ff2500,stroke:#333,stroke-width:2px
    style K fill:#b41a00,stroke:#333,stroke-width:2px
    style N fill:#ff664d,stroke:#333,stroke-width:2px
    style O fill:#ff2500,stroke:#333,stroke-width:2px
    style P fill:#b41a00,stroke:#333,stroke-width:2px
    style Q fill:#ff664d,stroke:#333,stroke-width:2px
    style R fill:#ff2500,stroke:#333,stroke-width:2px
    style S fill:#b41a00,stroke:#333,stroke-width:2px
{{< /mermaid >}}

