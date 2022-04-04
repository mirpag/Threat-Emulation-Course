# Reviewing the Windows System before the emulation

{% embed url="https://youtu.be/gf4EZb11akI" %}

Before we do our emulation, we're going to take a look at our Windows system to see what's there.&#x20;

1. On your Windows workstation, go back to your PowerShell ISE window.  `cd C:\users\[username]`Then `cd .\Documents` . Follow that with `dir`. There will be some test documents here.&#x20;
2. Run `dir --Recurse` to see all of the files. We will be changing some of these file names eventually.&#x20;
3. Run `Get-ComputerRestorePoint` to see if we have any restore points on the system.&#x20;
4. Run the following commands to get back to your desktop and list the directories and files: `cd ..`, `cd .\Desktop`, `dir`.
5. Lets take a look at our Windows Defender Settings. Open the application, and go to "Manage Settings". Ensure that the "Real-time protection" setting is on.
6. Scroll down to "Controlled folder access". This setting will allow you to add folders that you want to protect at default. You can add as many as you want to. Make sure this ability is turned on.&#x20;
