---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Why Threat Emulation?

You want to understand and detect the behaviors of threat actors and threat groups. What are their tools and techniques? The main purpose is for you to determine if you are able to detect that behavior and if your controls are in place that can mitigate their attack. We're going to talk about the nuances of that and and why threat emulation is necessary.&#x20;

### Why don't you just do a pen test?

Well, pen tests are typically a snapshot in time. You hire an organization, and they perform various activities like scans - all kinds of reconnaissance. Maybe you don't have a direct presence on the Internet, meaning you don't have ports open to your internal network. So they're going utilize spearphishing, for example. They're going to look for numerous vulnerabilities and exploit those, if possible, and see how far they can get into the organization undetected, they will write a report and give you some remediation steps to take. However, your existing controls may block their attempts.&#x20;

The pen test has, I wouldn't say limitations, but there are some aspects of it that the pen test doesn't cover and it's also over a period of time. So this could be a few days, maybe a week, and then they're done with their testing. And quite honestly, if your security controls block the pen testers, that's great, but they must stay within the scope of the pentest so there may be some tests they can't legally perform. You may even have specific systems that they can't access because it may disrupt production.&#x20;

A threat actor is not going to care that there is a system they can't test or can't log into, they're going to try it anyway. If that is their purpose or their motivation, that's important. Threat emulation is a continuous process. It allows you to perform exercises on a routine basis based on changes in your organization.&#x20;

If you are an MSSP (Managed Security Service Provider) that performs SOC capabilities for an organization, it's going to allow them to determine if you can detect specific adversary behavior that is known to target the type of organizations being monitored. If not, then you may need to add more log sources to monitor or train your analyst on how to detect those behaviors. The logs may be right there in front of them but didn't know the value of it.&#x20;

What are the pen tests? Once again, you're looking at specific techniques of the threat actors and the software they use. A pen tester may not be able to run certain tools because - like Mimikatz, for example, is used to dump hashes of password, and allows for lateral movement once they have the hash. If your systems are configured properly, Mimikatz won't be able to run so pen testers are limited in that capacity. However, a threat actor will do a lot of homework on your organization (so does a pentester, but the threat actor has much more time to analyze their target). They're going to learn what type of antivirus you use, what type of Endpoint Detection and Response (EDR) systems you have, learn about the employees and their roles, and they're going to start customizing their malware to evade those tools.&#x20;

So the pen test again, has a limitation of scope. With threat actors, there's no scope, anything goes. That's what you're planning and testing within your organization - the "anything goes" scenario.&#x20;
