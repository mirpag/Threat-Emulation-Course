---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjU5NDQzNA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Privilege Escalation

If they attack the system, they execute a PowerShell script. They want to maintain persistence, but the user is not an admin. What they're going to start doing is trying to escalate their privileges. By escalating their privileges, they're able to better maintain persistence. It may require admin access in order to install this software, so they need to maintain that access.&#x20;

![](../../.gitbook/assets/escalation.PNG)

They're going to go through a series of steps. One is just running a PS executable to see if they can log in as admin. They may look for Host Based vulnerabilities, or they may see, that a normal user has access to a script that they get started doing a reboot. If you start a script during a reboot, it's been a run with likely admin privileges. They can potentially inject themselves there if they are able to get into a login script of some way on a Linux system or Unix based system, for example. They're going to scan a system to look for the software installed, see if there's any vulnerable software that they can use to exploit, to then escalate privileges. You're looking at all the techniques that they may use, and all the sub techniques that may be used as well.

![](../../.gitbook/assets/escalation\_technique.PNG)
