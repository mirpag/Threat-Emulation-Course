---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Why Threat Emulation?

You want to understand and detect the behaviors of threat actors and threat groups. What are their tools and techniques? The main purpose is for you to determine if you are able to detect that behavior and if your controls are in place that can mitigate that behavior. We're going to talk about the nuances of that and and why threat emulation is necessary.&#x20;

### Why don't you just do a pen test?

Well, pen tests are typically a snapshot in time. You hire an organization, and they perform various activities like scans - all kinds of reconnaissance. Maybe you don't have a direct presence on the Internet, meaning you don't have ports open to your internal network. So they're going to go to utilize spear phishing, for example. They're going to look for numerous vulnerabilities and exploit those if possible, then print a report and give you some remediation steps to take. Your existing controls may even block their attempts.&#x20;

The pen test has, I wouldn't say limitations, but there are some aspects of it that the pen test doesn't cover. And it's also over a period of time. So this could be a few days, maybe a week, and then they're done with their testing. And quite honestly, if your security controls block the pen testers, that's great. But they are within scope, there's only some things they can do. There's some things they can't do. You may even have specific systems that they can't access because it may disrupt production.&#x20;

A threat actor is not going to care that there is system they can't test or can't log into, they're going to try it anyway. If that is their purpose, if that is their motivation, that's important. Threat emulation is a continuous process. It allows you to perform these exercises on a routine basis based on changes in your organization.&#x20;

Or if you are a MSSP that performs SOC capabilities for an organization, it's going to allow you to retain the test to see - here's a new threat actor, here's the new behaviors that they're exhibiting - can we detect those in our in the organizations that we're monitoring? And if not, then you may need to increase your log source reviews or train your analyst and how to detect those behaviors. The logs may be right there in front of you. But you didn't know that has some value, until you have threat intelligence to help guide that process.&#x20;

What are the pen tests? Once again, you're looking at specific techniques of the state actors and the software they use. A pen tester may not be able to run certain tools because - like Mimicatz, for example, is used to dump hashes of password, and allows for lateral movement  easily once you have that hash. If your systems are configured properly, Mimicatz won't be able to run. So pen testers are limited in that capacity. However, a threat actor will do a lot of homework on your organization. They're going to learn what type of antivirus you use, what type of Endpoint Detection and Response (EDR) systems you have. And they're going to start customizing their malware to evade those tools.&#x20;

So the pen test again, has a limitation of scope. With threat actors, there's no scope, anything goes. That's what you're planning and testing within your organization - the "anything goes" scenario.&#x20;
