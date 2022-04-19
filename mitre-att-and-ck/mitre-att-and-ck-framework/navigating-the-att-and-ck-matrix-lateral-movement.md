---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjY4ODE2Ng&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Lateral Movement

Lateral movement is when threat actors access other systems in the organization from the initial access point. That's what makes incident response and cleanup very difficult. You need to understand the behavior of the adversaries and what their tools are first, and then start to use tools and other resources to determine on which systems they reside.&#x20;

![](<../../.gitbook/assets/lateral movement.PNG>)

If you have 100 systems, the attackers will probably compromise about 10 of those just to maintain the access they want. It's not likely that they are going to compromise all 100 systems. But once it's been compromised, it's going to be virtually inactive until a given period of time.  The malware will then wake up and beacon out to the C2 server for instruction. This lateral movement is when mass compromises are, or do become a nightmare in the organization. These are the techniques that are used to achieve this goal of lateral movement.&#x20;

![](../../.gitbook/assets/lateral\_movement\_techniques.PNG)
