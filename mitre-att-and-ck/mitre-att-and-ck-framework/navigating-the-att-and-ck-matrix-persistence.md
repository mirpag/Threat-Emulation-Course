---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjU5NDQzNA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Persistence

The next thing that may happen, depending on the goal of the adversary, is persistence. Persistence is where they're trying to maintain access inside of the network. This is important because the adversaries goal may be something like find documents related to an acquisition or intellectual property. Once they find the documents, they're going to jump to exfiltration.  They may harvest credentials and persist or wait and capture email messages and documents and keep track of what the organization is planning, steal intellectual property, etc. **The Att&ck tactics are not linear***.

![](../../.gitbook/assets/persistence.PNG)

To maintain persistence, they're going to try to either determine if the current user is an admin. If they are, that's great. It makes persistence a lot easier (and lateral movement. That means they can run their malicious code, and maybe add a job into the test scheduler that runs periodically, and gives them a command shell remotely or exfiltrates documents, if needed. Below are some TTPs which are employed to maintain persistence. Ensure monitoring is being performed on new scheduled tasks and cron jobs or modifications to startup scripts, new services, and registry keys.&#x20;

![](../../.gitbook/assets/techniques\_persistence.PNG)
