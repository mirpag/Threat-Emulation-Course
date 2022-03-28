---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Threat Emulation Tools

* Caldera Mitre (free)
* Infection Monkey (free)
* Atomic Red Team (free, based on Powershell)
* Prelude (free and commercial)
* Scythe (commercial)

There are many more threat emulation tools out there than are listed above but these are some very popular ones.&#x20;

Caldera Mitre is what we're going to use for this exercise in this workshop.&#x20;

Don't get stuck on one tool because you want to understand what the tools capabilities are and your organizational needs. You'll see a lot of similarities, which makes it easier to move to a different tool because you're going to learn what capabilities to look for in threat emulation software.&#x20;

One that is most interesting in Atomic Red Team which are a collection of PowerShell scripts. In your test environment, within your organization, you're going to have to allow PowerShell scripts to execute. This can still work without having to allow PowerShell across the board, because you can use bypass mode, which means it's going to execute during that session. Though, you don't have to enable PowerShell scripts to execute throughout the entire organization.&#x20;

Scythe is a commercial tool and their website has lots of information about threat emulation.

Prelude is a spinoff of Caldera Mitre. It was a senior engineer who spun off and created Prelude, which is free but they also have a commercial option for additional plugins, which is around $50 a month. We're going to talk about why that may be optional or may not be an option, because you can also create your own emulation rules, using Caldera.&#x20;

Each tools allows you modify it based on your organizational needs, which is a very important feature. You're able to customize the threat emulation tools. This is one of the first features you want to look for. If you can't customize it, or if they give you a set in stone set of templates, I would suggest looking at other tools. Every organization is different, and has their own unique setup and capabilities.
