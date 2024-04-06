# NTFS-ADS
 NTFS hides extra data (ADS) in files, like hidden messages.


Step 1.
Create the "ADS.txt" file, write "This is my ADS file(or other words)",and save the file.

Step2.
 Open "cmd.exe", write the command "echo notepad.exe > ADS.txt:secret" in cmd.exe.

Step3.
Open "powershell.exe", write the command "Get-Content ADS.txt -Stream secret".
The terminal show "notepad.exe" strings.

Step4.
write the command "$e = Get-Content ADS.txt -Stream secret" and "Invoke-Expression $e".
 
Then screen automated show the notepad.
