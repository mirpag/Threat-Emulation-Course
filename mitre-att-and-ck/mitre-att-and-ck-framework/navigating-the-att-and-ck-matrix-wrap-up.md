---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjY4ODE2Ng&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Wrap-up

That covers the tactics that are used, and the goals of the threat actor activity. What are they trying to get? They may stop after they execute a command that searches a system for information. They zip it up, they exfiltrate it, and they're out of there. The malicious code may stay behind, or it may be set to automatically delete after reboot. The system they wanted, they were able to get it after their initial access, moved to execution (script that performs the discovery), discovery (search the host or shared drives), collection (stage the files in a directory and zip it), and exfiltration (remove the zip file from the organization).

TTP comes from - tactics, techniques and procedures. That's the Mitre Att\&ck framework. The way to look at this is to actually look at reports and start looking at the tactics associated with each one of them.

The Att\&ck Matrix is at [attack.mitre.org](https://attack.mitre.org).  They do provide an offline option for the att&ck framework, the entire attack.mitre.org site, including the search functions.&#x20;

In the next section, the Att\&ck navigator will be demosntrated in order to start learning how to create heat maps. Heat maps are the really the lifeblood of the Mitre Att\&ck framework. It documents the TTPs for a specific software program, or for a specific threat group.
