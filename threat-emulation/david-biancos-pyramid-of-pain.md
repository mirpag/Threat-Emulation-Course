---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# David Bianco's Pyramid of Pain

What drives threat emulation, is this great pyramid that David Bianco created, called the Pyramid of Pain.

![](../.gitbook/assets/David-Bianco\_Pyramid-of-Pain-v2.png)

Typically you hear it explained, that on the bottom, hash values can change really easily. So it's trivial to change those. However, it explains the pain that can be inflicted on the adversary and deny them the capability to evade your defenses, evade your security controls and your monitoring. At the bottom, hash values, those can change pretty quickly because if they use custom malware,  they can add a comment and the hash value changes. Any tools you have that are looking for specific hash values can be evaded.&#x20;

As a result, IP addresses can change because of fast flux DNS. For example, where they have a DNS record or Time To Live (TTL) record where it's going to change very rapidly. By the time you do a look up, the IP address that attacked you is very different than the domain that was seen in the logs.&#x20;

This is the same thing with domain names, those can change. You may see high entropy domains that are very cryptic and make no sense when you look at them. But those can change and any information about the domain holder can be hidden and unavailable to you.&#x20;

When we start getting into tools and network artifacts, that's where evasion becomes a bit more difficult for the adversaries to change. That's when you start inflicting serious pain. They're going to keep using the same tools or similar tools to help achieve their goal. In many cases, the adversaries are in an organization's systems for quite a period of time. They're able to update the capabilities, especially if they find a bug - in their own malware - and log in and update their tool within your system.&#x20;

At the very top, that's the really painful part for threat actors. Threat actors are humans.  Don't forget that they're people - they're groups of people. As a result, their behaviors often don't change. That's what TTP is Tactics, Techniques, and Procedures. We'll go into depth with that in the lesson on the Mitre Att\&ck matrix, tactics, techniques, and procedures.

If you've heard that word, essentially, it's the behavioral aspects of the adversary. They may change a tool, but it will probably perform the same task. As a result of TTPs, you can typically determine attribution. Who is the threat actor that's performing the attack? What are their motivations? What are they doing?&#x20;

You're going to see how to create a heat map of those behaviors. Then, you'll be able to test that against your existing capabilities. Even just using heat maps, you'll learn how to map out a threat adversary that already exists. Then you'll create some sample security controls and monitoring controls you can have in place. I'm going to show you how to take the information to determine if you can detect those behaviors of known threat actors.&#x20;

That's where it becomes very, very difficult and very painful for the adversaries. Once you know their behaviors, then it becomes much easier to detect and defend against them. Even though threat actors know that these TTPs and matrices exist, they're still successful with many organizations. Many organizations don't have the security controls or people to thwart their attack. They're still going to continue using those same behaviors and those same (or similar) tools. That's why tools and network artifacts are at the top of the pyramid because that starts to inflict pain on an adversary that can be very easily detected. The tools may change, but not the use and behavior of those tools and they produce very similar network and host artifacts, that makes them very easy to detect.
