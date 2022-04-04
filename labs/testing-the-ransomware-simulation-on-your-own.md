# Testing the Ransomware Simulation on your own

{% embed url="https://youtu.be/lT-ZCpw4XGQ" %}

1. You should be successful from your last test. Now, we have to remove that file association so we can run it with the full test. Open Command Prompt and your Default Apps.&#x20;
2. In Command Prompt, run `assoc .README=`.&#x20;
3. In the Default Apps window, scroll down. Click "Reset". The file association will be removed now.&#x20;
4. Delete the .README file and empty the Recycle Bin.&#x20;
5. Run this PowerShell test on your own:

```
get-childitem C:\Users\[user]\Documents -Filter "*pdf*" -Recurse | rename-item -NewName{$_.name -replace 'pdf','pysa' }
dir -recurse C:\Users\[user]\Documents
get-childitem C:\Users\[user]\Documents -Filter "*pysa*" -Recurse | rename-item -NewName{$_.name -replace 'pysa','pdf' }
dir -recurse C:\Users\[user]\Documents
```
