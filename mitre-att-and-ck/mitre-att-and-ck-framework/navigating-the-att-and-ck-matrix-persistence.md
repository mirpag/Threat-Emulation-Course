---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0NjU5NDQzNA&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Navigating the Att\&ck Matrix - Persistence

The next thing that may happen, depends on a goal of the adversary. This is persistence. Persistence is where they're trying to maintain access inside of the network. So they try to maintain a foothold. This is important, because the adversaries goal may be to find documents. Once they find documents, they may jump over to exfiltration.

![](../../.gitbook/assets/persistence.PNG)

Exfiltration, that means they're stealing documents out away from the organization. It may scan your computer for PDFs, Excel documents, Word documents, or any other file extensions that may have very sensitive information.

This is based on the reconnaissance phase earlier in the process. Their reconnaissance may help them know what information is that they want. They write malware that goes out and it finds it, zips it up, encrypts it, and maybe uploads it to their attacking servers. Exfiltration is stealing data from the organization.&#x20;

It's important to know because their goal may not be to have persistence. They may not care about that, because they got what they wanted. With persistence, this is an interesting one. This is where they're logged into the system. Let's say that it executes a PowerShell script. And that PowerShell script then goes out and downloads the main payload. That PowerShell script may be, one or two commands that goes out, downloads the main payload, and executes it. That can be a visual basic script. It can be a Python program. It can be one of these execution sub-techniques that we see right here.

![](../../.gitbook/assets/techniques\_persistence.PNG)

Persistence, they're going to try to either determine if the current user is an admin. If they are, that's great. It makes persistence a lot easier. That means they can run their malicious code, and maybe add a job into the test scheduler that runs periodically, and gives them a command shell remotely, if needed. What you're looking at here are the various techniques and sub-techniques that are used to maintain persistence. Be sure you take a look through these scheduled tasks. This is a big one. As security admins, you want to be sure that you keep an eye on any new or removed scheduled tasks on all your systems.&#x20;
