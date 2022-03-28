---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Threat Emulation & Threat Intelligence

The threat emulation plana and process are developed based on intelligence resources. That's why you want to ensure that you're extracting the relevant information from your sources. Ensure that it has been disseminated from a reliable and trusted source. If possible, have a mechanism to provide feedback. Your plan is based on either threat intell from an external report or - especially for a SOC analyst - you may know of threats going on that target a specific organization. With that information you have based on the logs and the behavior you are detecting, you can create a heat map, apply that and create a playbook.

Threat intelligence is really important for threat emulation, because you are able to mimic the behaviors of the adversary. It really depends on how you choose to perform the threat emulation exercise; you can take systems and offline and set up a network but you want to be absolutely sure that the offline network looks just like the network that you're trying to protect against.

Here's a nuance with that: if you're in a SOC, you can't duplicate every single organization you're monitoring, because it may be dozens of organizations and it may consume a significant amount of time. However, there can be a test lab where behaviors are emulated and then the SOC analysts can learn the behaviors to look for in the logs AND determine if their SEIM can detect the behavior.&#x20;

For those who are doing this within the organization, a couple of ways you can do this includes offline. You have the domain server, and four or five systems that are set up and configured exactly like your organization of computers. That's really, really important. You want to be sure they look like and are configured with the exact same controls as hosts within your network so that you know how your controls are going to behave. The other method is based on the emulation exercise, on TTPs, the behavior of the threat actor, and the destructive and non destructive means, where you run the threat emulation exercises on your real systems.&#x20;

What you're going to see with Caldara, Infection Monkey, Prelude, etc. is that you're going to deploy an agent on your systems, which simulates a C2 connection. Then you perform a series of steps to collect information, perform actions on that computer, attempt lateral movement in the organization, etc. That will allow you to see how your hosts repond and if the controls you have, or the organization you're monitoring controls, are in place and working as expected.