# Test File Association for README that the ransom creates

{% embed url="https://youtu.be/HxmGM-f1jXk" %}

1. On your windows machine, open up Command Prompt. Run this as an administrator.&#x20;
2. Run `cd C:\Users\[user]\Desktop`. Run `dir.`
3. Run `echo test > Read.README`. A file will appear on your Desktop. Once you open the file, you can see that "test" is written inside.&#x20;
4. Open the Windows search bar and search "Default Apps". Click to open. Once this window is open, scroll down to the bottom of the window and click "Reset".&#x20;
5. When we did this, this didn't end up getting rid of the association, so we will run a command in Command Prompt to make this work. In Command Prompt run, `assoc .README=`.
6. Now we can go back to our "Default Apps" settings and click "Reset". The association should be gone now.&#x20;
7. In Command Prompt, run the following command: `echo Your files are encrypted. To get all your data back contact us: test@protonmail.com > Read.README`.
8. To see the text written in the .README file, run `type Read.README`.
9. Right click on the file to delete. Then, right click on the Recycle bin and empty it.&#x20;
