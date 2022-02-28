---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Detecting & Emulating Behavior

For detecting behavior, as your controls work and block the attack, make a note of that. Then create a playbook so you know and learn how to detect that quickly. Create playbooks that can look for the activity, and alert you to say: "we noticed XYZ threat active behavior", so it's very specific to you. What is actually going on? Then you remove that control, and then emulate a little bit further until you get to the the ultimate goal.&#x20;

Your event recording devices, logs, SEIMs, EDRs, and any kind of intrusion detection systems you have are probably lit up. If not, that's fine as well. If you want an exercise with 20 steps, and you want to detect five, that's fine. You now know you need to configure your systems to detect the other 15. It's just how that is.&#x20;

If you don't know who your threat actors are, and if you're just monitoring to be monitoring for the most common stuff - that's one thing. You're going to see with Caldera Mitre that as its performance is threat emulation, it can emulate a simulate behavior of a regular user. It looks just like normal user behavior. So it's hard to detect. That's something that adversaries really do. They will attack your network while you're working during the day so activity doesn't look so abnormal. Your logs and your Sims are going to be, tested, essentially.&#x20;

For SOC analysts and SOC shops, this are really good exercises. It helps you to see what your current tools are capable of, and what you need to enhance. By learning through emulation, you're adding value not just to your own learning, but to the organizations that you're monitoring. You're providing value to them as well by increasing the monitoring capabilities and the services you're providing and being able to create playbooks that have threat actors that target specific organizations.&#x20;

So, again, don't get discouraged if your tools don't detect everything. Now you know what it is not capable of and you can change that. That's the important part. You can change that behavior.&#x20;

We'll look at some tools that you can use to help with increasing the auditing capabilities in your organization. Sis Mon, is a very useful tool. It is a driver you install on Windows systems. It provides very little overhead, or creates very little overhead for the overall system. You can set up something like an x log, or log B, to send those sis mon events to a remote system. You can then create playbooks out of that. When you see someone using NET view, net use, or other net commands in rapid succession, then you can say: "this is unusual behavior". That's a playbook that you can create. If you see those tools being used, if you see bits admin being used, there's something weird going on with your system, because it's not used very often. These threat emulation exercises are going to be highly beneficial for your organization and your customers.
