---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHx0ZWNofGVufDB8fHx8MTY0NTk5MDg4Mg&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Detecting & Emulating Behavior

For detecting behavior, as your controls work and block the attack, make a note of it. Then create a playbook so you know and learn how to detect that quickly. Create playbooks that can look for the activity, and alert you to read: "Potential XYZ threat actor behavior", so it's very specific to you. Then you remove that control, and then emulate a little bit further until you get to the the ultimate goal.&#x20;

Your event generating devices, logs, SEIMs, EDRs, and any kind of intrusion detection systems you have are probably lit up. If not, that's fine as well. If you run an exercise with 20 steps, and detect five, that's fine. You now know you need to configure your systems to detect the other 15.&#x20;

You're going to see with Caldera that as it performs the threat emulation exercises, it can simulate behavior of a regular user (if the plugin is enabled). That's something that adversaries do. They will attack your network while you're working during the day so activity doesn't look abnormal.&#x20;

For SOC analysts, these are really good exercises. It helps you to see what your current tools are capable of detecting, and what you need to enhance. By learning through emulation, you're adding value not just to your own learning, but to the organizations that you're monitoring. You're providing value to them as well by increasing the monitoring capabilities and the services you're providing and being able to create playbooks for threat actors that target specific organizations.&#x20;

**Again, don't get discouraged if your tools don't detect everything. Now you know what it is not capable of and you can change it.**.&#x20;

Some tools that you can use to help with increasing the auditing capabilities in your organization include Sysmon which is very powerful. It is a driver you install on Windows (and now Linux) systems. It has very little overhead on performance. You can set up something like nxlog, or your existing EDR agent, to send the Sysmon events to a remote system, such as a SEIM. When you see alerts on someone using *net view*, *net use*, or other *net* commands in rapid succession or based on known usernames by threat actors, then you can say: "this is unusual behavior" or if the admins don't usually use those tools then that would be a trigger. 

Threat emulation exercises are going to be highly beneficial for your organization and your customers.
