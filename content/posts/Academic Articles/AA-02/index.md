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
mermaid: true
---

The following is an informal explanation of my thesis study. For a more formal reading, [here](https://www.proquest.com/openview/0aa707187ddd21fcf5a9ea1b847cb278/1.pdf?pq-origsite=gscholar&cbl=18750&diss=y) is a link to the published version. This written piece will cover what the study was about, the study design, why it may be important and future research directions. 

---

## The Problem:
In industry and academia practitioners who work with any human movement data often rely on some sort of digital human modeling software in order to do any kind of analysis or simulation.  Various studies had shown that this software had been inadequate and could be improved upon in various ways.  
Specifically for engineers in the automotive manufacturing industry, the software was limited to analyzing only a single static posture and maybe a few rudimentary dynamic ones. This restricted their ability to fully assess the injury risk associated with complex aspects of manual assembly operations.


## The Solution:
We wanted to improve the process of creating full workstation simulations through digital human modeling. The study was designed to understand motion behavior with the intention of modeling the motions specific to specific automotive manufacturing tasks in the future. This would help industry engineers from having to manually create human simulations.  Also, it would improve simulation accuracy as kinematic data could be collected on those performing actual tasks within the work environment.


### Why do we care about movement variability?

Typically in human movement, there are normal variations that occur within a (healthy) individual during motor performance across multiple repetitions of a task and it is nearly impossible for an individual to perform two identical actions of the same task. It's been describe by various researchers as "repetition without repetition".  

As individual exhibits some sort of natural variation within their movement that is unique to them, this can be thought of as a person's natural variability profile.  Once we have someone's natural variability profile, we can then compare and contrast between individuals and maybe even come up with some aggregate explanations for different groups. More broadly, this could help us to understand the rules of motion that humans use to base their behaviors during specific tasks.


### What is time series analysis?

Other work in the past has reduced available time series data down to a single 0 dimensional variable that would describe the dataset as a whole (i.e local max, local min, area under curve…etc). The problems with this approach is that it reduces down data to something that may not even describe what you initially intended to. 

In order for us to do any robust analysis of movement, we needed to collect data and extract a meaningful summary of continuous movement. That is pretty much what time series data is…just an observation with a time component. In the case of my thesis, the observation was joint angle over a series of time points.



## Study Design 

### How did we setup the study?

We decided compare the movement of individuals of different percentile height groups. We defined percentile height groups from the ***NHANES 2011-2014*** (the most recently available height dataset at the time) dataset which we thought would be a decent approximation of North American height distributions. The following image demonstrates the various male and female height percentile distributions:
 *** Add in charts….if charts don't work, add in distribution plots ***

Twenty participants completed seven simulated automotive assembly tasks commonly found in industry. The 20 participants were evenly distributed into 1 of 4 groups based on their height. So (7 Tasks × 7 Joints ) = 49 levels of analysis. It should be noted that we didn't take into account gender, only height distribution. 


### What did we find?

Well based on the results, every group in the study performed each task with a unique multi-joint coordination pattern. Simply put, not two groups shared an identical set of joint angle profiles. Well it's actually more complicated than that, but if you want the complicated answer checkout my thesis publication ***here***.  Generally, we did find that the closer in height groups were, the more similar their joint coordination profiles. 

