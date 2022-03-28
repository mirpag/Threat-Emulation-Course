# Deploy First Agent

{% embed url="https://youtu.be/kzK_18pR4Pw" %}

1. Open up Firefox on your Linux machine. Connect to localhost:8888. This is where Caldera is being hosted.
   1. Username: admin, Password: admin
2. Once you are logged in, we are going to create our first agent. Click on the 'agent' section on the left-hand side of the screen.&#x20;
3. Click on 'Deploy an agent'. In the 'Choose an agent' section, select the GoLang agent. This will be for the Windows platform.  This will then create a PowerShell script to create an agent for your Windows system.&#x20;
4. In the text box next to app.contact.http, add the IP to your Windows server. It will update in the script.&#x20;
5. Copy the PowerShell script to your clipboard using the 'Copy' button.  Move to your Remina desktop and open Windows PowerShell ISE. Run this as an administrator.&#x20;
6. Paste in the scripting environment.&#x20;
7. Run the script. This may take a few moments to initialize. Pay attention to where this is being installed! If you get a pop-up, click the 'Allow Access' option.&#x20;
8. Go back to Caldera, and close the 'Deploy an agent' window. Go to the 'agents' section on the left-hand side of the screen again. &#x20;

Now, you should see that you have a new Windows agent in this section!
