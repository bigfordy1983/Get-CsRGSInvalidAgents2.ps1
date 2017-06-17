# Get-CsRGSInvalidAgents2.ps1

This is a Skype for Business Powershell script designed to clean up "Ghost" users who have been disabled but still appear in Response Groups.

This Script is a modification of the rather excellent original script by David Paulino http://blogs.technet.com/b/uclobby/
It improves the runtime by storing a get-csuser to a variable and calling the variable in the for-each loop, rather than running cs-user on each loop.
This script runs itself, it has two Parameters, -Name where you can specify the name of a specific Response Group and -Remove which automatically removes the user from the response group

To run, just run the script.
