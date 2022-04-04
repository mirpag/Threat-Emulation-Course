---
description: (You are going to run your own operation with this)
---

# Create File Association README Ability

{% embed url="https://youtu.be/6AxKdVFh5Qo" %}

1. In Caldera, your agent status will most likely be "dead, untrusted". Let's fix this. Go back to your Windows machine.
2. In Command Prompt, run `cd C:\Users\Public`. This is where our agent is located.&#x20;
3. Run `sandcat.go-windows.exe -server http://10.0.5.55:8888 -v` to start your agent.  In Caldera, your agent will now be up and running.&#x20;
4. Go to the "Abilities" section in Caldera. Click on "Create an Ability"
5. Call this ability "Change File Association". For the description, write "Changes the .README file to be associated with text files".
6. The tactic will be "execution". The Technique ID will be "T1059.003". The Technique Name will be "Command and Scripting Interpreter: Windows Command Shell".
7. Scroll down. Change the platform to "Windows". Change the executor to "cmd".
8. The command will be `echo Your data is encrypted. Contact us to get your data back! > C:\Users[user]\Desktop\READ.README && assoc .README=txtfile`.
9. The timeout will be "10". Click "Save" & "Close".
10. Move to the "Adversaries" section in Caldera. We are going to add this ability to the PYSA Sample Emulation adversary we have been creating. Be sure to select the correct profile.&#x20;
11. Click "Add Ability" and search for "Change File Association". Notice that this doesn't show up.&#x20;
12. Close this window, and refresh this page. Click on "Add Ability" and search for "Change File Association". This will now show up. Click "Save and Add".
13. Click "Save Profile".
14. Now, try to run these particular tests. Then, login to your Windows system to see if your file was created and the association was created. Go to "Operations" and create a new operation. Make sure your agent is alive and trusted, and run your operation. &#x20;
