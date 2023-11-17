1/c Lauren Oakes 

Computer and Network Security 

16 Nov 2023


# Mimikatz 
Mimikatz is a Windows explotation (meaning its used against Windows machines) tool that can grab passwords and other sensitive info by digging into a computer's memory. This information can be anything from usernames and passwords to various certificates. It works by gaining access Window's LSASS or Local Security Authority Subsystem Service that handles all of this data then extracts it. But it only works on Windows because of Windows specific vulnerabilties when it comes to Windows authentication data, other operating systems don't work exactly the same way so a different tool will be neccesary to exract the same kind of information. This tool can be downloaded on github as a zipped file containing both 64 and 32 bit versions. However, because of the nature of this tool, and it's specific Windows target, Windows really does not like it when you try to download this tool because it opens the machine up to a lot of vulnerability just by being downloaded. Overall, this tool can be used by security proffesionals to find and fix system vulnerabilities, but it can also be misused by attackers to steal information and is therefore inherently a very pwoerfl but easy to use tool with lots of available documentation online.For more information including specific screenshots and directions on how to use mimikatz, please refer to the following section.

# Demonstrate Mimikatz use - Difficult
To begin this attack I first decided that I wanted to use my Parrot OS VM to attack my own Windows workstation (mainly becasue I couldn't access my Windows VM's beacsue of a password reset issue). Once in Parrot, I located and installed mimikatz (https://github.com/gentilkiwi/mimikatz/releases) and unzipped the file locally.

Next, I had to figure out how to get my mimikatz file onto my Windows workstation. So I created a scenario where an attacker happens to know the password to one account on the system is (perhaps a phishing attack, disgruntled employee, or pure social engineering). I don't believe a password would have been necesary if I was attacking my Windows VM because it has less secuirty in place. However, I used this password to use scp and transfer my malicious file to my Windows Workstation as seen below.

![](https://github.com/LaurenMOakes/Oakes_CNS/blob/main/HW8/scp.png?raw=true)

Now, I knew I needed to run the mimikatz.exe deliverable I had just transfered, so using the password I knew from the scenario above, I ssh into the Windows Workstation and ran the file. This was only possible becasue I knew exactly where I put the file from my scp command. From there I knew I had to escalte my mimikatz privileges (or at least check they were at the correct level) or I would be restricted from running some commands, this is seen below.

![](https://github.com/LaurenMOakes/Oakes_CNS/assets/90365484/d06fa1e3-fac7-4b03-b999-ee6f8ddc3a87)

Finally, I experienced with running some commands and playing around with what I could extract from my Workstation. Seen below are some succesful commands I ran and what they mean.

This one simply returns a list of all the tokens from the work station:

![](https://github.com/LaurenMOakes/Oakes_CNS/blob/main/HW8/token_list.png?raw=true)

This one returns lots of cool cryptography information like hash algorithms, key types and sizes that could be used for future attacks:

![](https://github.com/LaurenMOakes/Oakes_CNS/assets/90365484/e714f19e-a775-44ea-8b1c-1ec4c5eda314)

Lastly, this dumps a list of every user on workstation and associated basic info, which is cool becasue I didn't even know some of these users existed on the workstation:

![](https://github.com/LaurenMOakes/Oakes_CNS/blob/main/HW8/lsadump.png?raw=true)



