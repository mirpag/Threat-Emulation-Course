---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjU5NDQzNA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Reconnaissance&#x20;

Reconnaissance or recon is gathering information to prepare to carry out their goal.

![](../../.gitbook/assets/Recon.png)

Here are some recon techniques.&#x20;

![](../../.gitbook/assets/techniques.PNG)

The TTPs here are active scanning, scanning IP blocks, vulnerability scanning, etc. This is where they are using tools or they are using search engines like Google to find out as much information as they can about their target. If they get enough information, it is very likely that the attack will succeed. With every single technique, you have a description of what it means. Then you have more links. You have a lot of links here to other information, this can go deep, deep, deep into the behaviors of the adversary. But you don't want to get caught in a in a loop, or diverge too far from what you're trying to try to understand and document about the adversary.&#x20;

Every tactic has an ID. When writing a report about the behavior of software, a threat group, their techniques, etc. the ID is placed next to the technique because it provides a common language for security analysts to understand the behavior. Every technique also has an ID as you see below for T1595, the technique for active scanning.

![](../../.gitbook/assets/id.PNG)

 Now each technique can have sub-techniques. With active scanning, a sub-technique is scanning IP blocks. The ID for that is T1595.001 as seen below.
 
 Active scanning is a sub-technique of T1595. T1595 is a TTP for the tactic reconnaissance.

![](../../.gitbook/assets/active\_scanning.PNG)

PRE and reconnaisance may not be mapped in a report. If they know how they were performing reconnaissance and if they know how they were performing resource development, it may be documented. It's okay to leave these two out when you're mapping the attack.&#x20;

![](../../.gitbook/assets/pre.PNG)

**Data source**
This is where the attack framework has real power here. It provides more than just "this is reconnaissance." This is how they perform reconnaissance. This is the technique where we get into how do you actually detect it. If you have a data source like network flow traffic, that's how the behavior can be detected.  There are many scans that occur on a network so trying to figure out the known threat actor may not be feasable. For SOC analysts, this part is really, really important, because they can determine if they have these capabilities of monitoring within the organization to help support incident responder analysis. *Network traffic flows can provide a lot of information*.

![](../../.gitbook/assets/data\_source.PNG)

Another benefit to the Att\&ck framework is that they show mitigations. Active scanning is difficult to mitigate depending on the type of scan being performed.&#x20;

![](../../.gitbook/assets/mitigations.PNG)

In the event of a compromise the logs could should the same IP traced to the attack performed some type of scanning in the past.&#x20;

![](../../.gitbook/assets/detection.PNG)

