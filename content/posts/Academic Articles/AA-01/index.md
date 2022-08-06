---
title: "Tools and Torque"
date: 2020-06-08T08:06:25+06:00
description: Sample post with multiple images, embedded video ect.
menu:
  sidebar:
    name: Tools and Torque
    identifier: AA-01
    parent: Academic Articles
    weight: 101
hero: power_tools.png
tags: ["Markdown","Content Organization","Multi-lingual"]
categories: ["Basic"]
mermaid: true
---

The purpose of this piece is to provide an informal explanation of this study as well as it's implications to industry and potential future research directions. Since the study was privately funded, much of the data and results cannot be presented publicly.  However, I will be examining the insights that I took away while conducting this study.

---

## The Project

### What was the study about?

Before diving into the study and the reasons for it, there's a few key terms that have to be explained. I'll begin by giving the formal purpose of the study, then start informally breaking down why each component of the purpose matters. 

> The purpose of this study was to compare the physical demands associated with the **right-angle power tool (RAPT)** operation when using Cleco’s Low Torque Reaction (LTR) and Bosch’s ERGOSTOP fastening strategies during simulated tightening of **hard and soft joints**.

#### What is a right-angle power tool?

Right-angle-power-tools (RAPT) are used in the manufacturing industry for joint fastening.  They have long handles which are perpendicular to the spindle-head.  When operating at higher torques, they provide a greater mechanical advantage when compared to pistol-grip power tools or in-line power tools. 

{{< video src="_cleco.mp4" >}}

Video clip of a participant performing a joint fastening.
{{< vs 3>}}


#### What are hard and soft joints?

{{< img src="hard_and_soft_joints.png" height="300" width="350" float="right" title="Hard and Soft Joints" >}}


The main difference between the joint types is comprised of the angular displacement each joint has to sustain in order to be considered fully fastened.  Generally hard joints require a much lower angle of rotation to reach target torque (target tightness) when compared to soft joints. This study required that the target torque was to be completed with an angular displacement no greater than 90° for hard joints and the target torque completed with an angular displacement no less than 360° (with no greater than 720°) for a soft joint.

In industry, hard joints typically fasten together metal to metal parts and soft joints fasten gaskets or spring washers. 
{{< vs 3>}}


#### Why do we care how joints are fastened?

{{< img src="torque_power_curve.PNG" height="300" width="350" float="left" title="Torque-Power Curve Example" >}}

Each company usually has some sort of patented fastening strategy implemented in their power tools. Well what does it mean to have a fastening strategy…?  Some companies could start of with a really high torque then slow down once they're approaching target torque…. others could slowly ramp up the torque until target is reached…… others could just go all out from the get go until target torque is reached.  There's generally many approaches companies can take to speed up or slow down tool torque to achieve target torque and fasten the joint. This is usually done by adjusting the angular speed (rotations per minute RPM). Torque refers to the capacity to do work, while power is the rate of completing work in a given amount of time. The primary use of torque is to make the spindle accelerate in the initial stages of movement, while the power determines the rate of the acceleration of the spindle.
{{< vs 3>}}




## Study Design 

### So how did we setup the study?

We brought in 20 participants (10 male and 10 female).  We wanted each person to try out each tool with a hard and soft joint. Also, we wanted each person to try out each tool at 3 different target torques 30 Nm, 55Nm and 75Nm. So (2 tools × 2 joint types × 3 target torques) = 12 conditions.  For each condition, every person performed a joint fastening every 12 seconds for a 5 minute period.  After each 5 minute period, each person was given a 3 minute break and asked to fill out a Borg questionnaire which asked about their perceived exertion and discomfort from a scale of 1-10. All trials were randomized, so the order in which the participants performed each fastening was not consistent.

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


As mentioned earlier, I really can't dive into the results or data. But although each tool accomplished the same job (tightening the joint) there was definitely a different feel to each one and every participant reacted to this in a unique way.


### Implications to Industry

So what did this study mean to industry practitioners? Well this study could be seen as a version of an A/B test. Simply put, with all things kept the same, which tool did participants prefer to use? Suppose tool A is decided, now we install tool A in our plant. But there are some issues that come with this, suppose tool A is 10× more expensive than tool B.  Should the company just eat the cost of tool expense to please their operators? What if tool A requires more maintenance than tool B? As you can see, many other factors come into play when deciding upon which direction to go.

Another interesting aspect to all this is the following. Just because participants prefer to use tool A compared to tool B….. Does that mean tool A is better for each person (in-terms of injury prevention) when compared to tool B? There are countless examples of products in industry that customers prefer but aren't necessarily the best for their health. This often leads to a business being left with an interesting ethical dilemma….do we make more money and sell the product that isn't the best for our customers but they really like? Or do we make less money selling the product that is the healthiest option for our customers but leaves them less satisfied.  Not all problems are this black and white but the general theme of the underlying problem exists.

In the case of this study, there were various metrics that were used to calculate injury risk of the individual. However, a company can't know definitively how many injuries will be incurred until the product is deployed into the workstation.  


## Future Research Directions

After completing this study, there were certainly many more questions that I had and many more elements that I wanted to explore.  

One of these was the physical characteristics of each participant such as height, weight, age, and grip strength that would have played a role in how they interacted with each tool. It would be interesting to probe whether the effects of these characteristics were negligible or if they played an important role. Personally, I believe that they do play a role… to what extent? I don't know.  But the implications could mean potentially being able to customize a workstation fully to an individual's characteristics.  Does person A have a tighter grip strength? Let's ramp up the torque! Is person B a taller individual? Let's change the tightening strategy to one that suits his height!

Another interesting area to explore has to do with the Borg questionnaire which are the subjective ratings each participant evaluated each tool/condition on. The fact that each participant knew which condition they were evaluating (i.e 30Nm Bosch Soft joint vs 75Nm Cleco Hard joint) meant that they had an idea of what joint should be more difficult to fasten compared to another. This would have definitely had an impact of their perceived exertion rating.  So perhaps a single-blind study design would have helped to reduce that bias. 



## Concluding Thoughts

Overall, I enjoyed performing this study as it was the first time I was set to be in charge of a whole project. I definitely had my challenges but ultimately I was able collect, analyze and report out the data collected in a manner that was adequate for our industry partners. 