# Running the 'Full' Threat Operation

{% embed url="https://youtu.be/tCRV1RIXr7k" %}

Hopefully you were able to run your PYSA Ransomware Test ability. It is likely that you got an "Access Denied" error due to your control folder access. In order for this to work properly, we have to configure the agent. Make sure to start that agent again!

1. Under the "Adversaries" section, check to see if your "PYSA Ransomware Test" ability is similar to the one showed in the video.&#x20;
2. Browse through the profiles that are available to you through Caldera. There are many abilities you can add to your adversary within these profiles.
3. Back in our "PYSA Sample Emulation" adversary, add another ability. Search for "Discover local hosts". Save and add this ability.
4. Ensure that your "PYSA Ransomware Test" ability is added as well. Save this profile.&#x20;
5. Add another ability. Search for "Disable Windows Defender All". Save and add.&#x20;
6. Add another ability. Search for "Windows - Delete Volume Shadow Copies". Save and add. Save the profile.&#x20;
7. We ordered our abilities like so:
   1. Disable Windows Defender All
   2. Change File Association
   3. Change Logon Legal Warning
   4. PYSA Ransomware Test
   5. Discover local hosts
   6. Windows - Delete Volume Shadow Copies
8. Let's run our operation! Go to the "Operations" section in Caldera. Click "Create Operation".
9. Our operation will be called "Run PYSA Emulation". Our Adversary will be "PYSA Sample Emulation". Make sure to click on the "Auto Close Operation" setting. Save the operation.&#x20;
10. Run this operation. At this time, you can look at your Windows machine to see if any pop-ups show.&#x20;
11. When we ran this, it looked like our antivirus killed our agent. But, after waiting a few seconds the agent came back on. The antivirus was disabled. You have to be patient with this!
12. Our "Discover local hosts" ability failed, due to the file not existing at the time the ability was run. This file must have been removed in an earlier ability. But overall, everything worked as expected!
