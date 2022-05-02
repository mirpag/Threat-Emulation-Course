---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# David Bianco's Pyramid of Pain

What drives threat emulation is this great pyramid that David Bianco created, called the Pyramid of Pain.

![](../.gitbook/assets/David-Bianco\_Pyramid-of-Pain-v2.png)

Bianco's Pyramid of Pain explains the pain that can be inflicted on the adversary and deny them the capability to evade defenses and monitoring. 

At the bottom, hash values, those can change pretty quickly because if threat actors use custom malware, they can add a comment and the hash value changes. Detection methods that check for indicators of compromise (IOC) such as hash values can be evaded.  It is very little cost to the adversary to change the tool which causes its hash value to change.&#x20;

IP addresses also are incur little pain and cost to an adversary because those can change frequently.  That can be see with evasion techniques like fast flux DNS. For example, where they have a DNS A record and aTime To Live (TTL) record set very low and the IP changes often when performing a forward lookup. By the time the analyst performs a lookup, the IP address that attacked their organization is different than the IP that was seen in the logs.&#x20;

This is the same thing with domain names, those can change. Adversaries may use high entropy domains that are very cryptic and make no sense when read, but those can change and any information about the domain holder can be hidden and unavailable to you.&#x20;

Tools and network artifacts are when it starts to incur a bit of 'cost' to the threat actor and it may start to become difficult to hide their tracks. That is when evasion becomes a bit more difficult for the adversaries to change. That's when pain is inflicted on teh adversary.  By using the same (or similar) tools and techniques, they leave behind evidence that makes it possible to attrribute the behavior to a specific threat actor or group. Artifacts like malware, scripts, registry entries, methods of performing tasks, usernames created, etc. incur a high cost to an adversary to change their behavior.&#x20;

At the very top, that's the really painful part for threat actors. Threat actors are humans.  Don't forget that they're people - they're groups of people. As a result, their behaviors or their Tactics, Techniques, and Procedures (TTPs) don't change much because it would require significant 'cost' to redevelop all of their malware, c2 servers, and behaviors.  Their goals tend to stay the same so their behaviors aren't likely to change, especially when their campaigns are so successful.

That's where it becomes very, very difficult and very painful for the adversaries. Once you know their behaviors, then it becomes much easier to detect and defend against them. Even though threat actors know that these TTPs and matrices exist, they're still successful with their campaigns. Many organizations don't have the security controls or people to thwart their attack. They're still going to continue using those same behaviors and those same (or similar) tools. That's why tools and network artifacts are near the top of the pyramid because that starts to inflict pain on an adversary that can be very easily detected. The tools may change, but not the use and behavior of those tools and they produce very similar network and host artifacts, that makes them very easy to detect.
