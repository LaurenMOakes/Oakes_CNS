1/c Lauren Oakes 

Computer and Network Security 

16 Nov 2023


# Mimikatz 
Mimikatz is a Windows explotation (meaning its used against Windows machines) tool that can grab passwords and other sensitive info by digging into a computer's memory. This information can be anything from usernames and passwords to various certificates. It works by gaining access Window's LSASS or Local Security Authority Subsystem Service that handles all of this data then extracts it. But it only works on Windows because of Windows specific vulnerabilties when it comes to Windows authentication data, other operating systems don't work exactly the same way so a different tool will be neccesary to exract the same kind of information. This tool can be downloaded on github as a zipped file containing both 64 and 32 bit versions. However, because of the nature of this tool, and it's specific Windows target, Windows really does not like it when you try to download this tool because it opens the machine up to a lot of vulnerability just by being downloaded. Overall, this tool can be used by security proffesionals to find and fix system vulnerabilities, but it can also be misused by attackers to steal information and is therefore inherently a very pwoerfl but easy to use tool with lots of available documentation online.For more information including specific screenshots and directions on how to use mimikatz, please refer to the following section.

# Demonstrate Mimikatz use - Difficult
