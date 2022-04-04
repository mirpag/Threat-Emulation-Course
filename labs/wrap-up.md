# Wrap Up

{% embed url="https://youtu.be/qKuszwShb3A" %}

Where do we go from here? We can go to the "Debrief" section of Caldera to see how the attack carried out. We can download the report as a PDF or JSON file.&#x20;

Now that we have this report file, we can work through this exercise with our Red and Blue teams to see what was successful, what commands were run, etc.&#x20;

The next portion assumes you have Sysmon installed on your Windows machine, and you have run the full threat operation.&#x20;

1. Within your Windows Machine, open up the Event Viewer application. Go to the "Applications and Services Logs". This may take a few to load.&#x20;
2. Go to the Sysmon folder. (Applications and Services\Microsoft\Windows\Sysmon)
3. Once you open up the Operational logs, you can see all the events. Move through this to see if you can find any evidence of the commands that were run through the threat operation.&#x20;
4. Use "Find" to search for "vsadmin". The command that was run by Caldera should show.&#x20;

Go through and see if you can find any other commands that were executed by Caldera!
