---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Threat Emulation & Threat Intelligence

The threat emulation plan and process are developed based on intelligence resources. Ensure that threat intelligence reports are disseminated from reliable and trusted sources. If possible, have a mechanism to provide feedback. The emulation plan is based on either threat intell from an external report or - especially for a SOC analyst - you may know of threats going on that target a specific organization. With that information you have based on the logs and the behavior you are detecting, you can create a heat map, apply that and create a playbook.

Threat intelligence is really important for threat emulation, because it describes the behavior to be emulated. The emulation can occur on production systems or a virtual network that mimics the production systems.  It is important the virtual network mimics as close as possible, the production environment.

Here's a nuance with that: if you're in a SOC, you probably can't duplicate every organization being monitored, because it may be dozens of organizations and it may consume a significant amount of time. However, there can be a test lab where behaviors are emulated and then the SOC analysts can learn the behaviors to look for in the logs AND determine if their SEIM can detect it.&#x20;

For those who are doing this within the organization, a couple of ways emulation can be done includes offline. You have the domain server, and four or five systems that are set up and configured exactly like your organization. That's really, really important. You want to be sure they look like and are configured with the exact same controls as hosts within your network so that you know how your controls will respond. The other method is based on the emulation of threat actors and the destructive and non-destructive behaviors where you run the threat emulation exercises on production systems.&#x20;

With many threat emulation platforms such as Caldara, Infection Monkey, Scythe, Prelude, etc. is that an agent needs to be deployed on systems which emulates malware communicating with a C2 server, which is the host where the threat emulation software is deployed. connection. Then you perform a series of steps to collect information, perform actions on that computer, attempt lateral movement in the organization, etc. That will allow you to see how your hosts respond and if the controls you have, or the organization you're monitoring controls, are in place and working as expected.