# Navigating the Att\&ck Matrix - Defense Evasion

Advanced threat actors often have the goal of evading defenses. If they're able to gain admin privileges, then they can start disabling services like Windows Defender or EDR software in order to prevent from being detected once they download the main payload to achieve their goal.&#x20;

The defense evasion methods you see here are methods they can use to prevent from being identified. Stopping the antivirus program is, is pretty egregious, because if the organization has monitoring software, they can tell the antivirus was stopped or uninstalled. What adversaries will do is find out what type of anti virus the organization has, or EDR they have, and then write the malware and test it against it - within the adversaries environment - to determine if it can detect it or, with admin privileges, they can have antivirus or EDR programs ignore their malware.
