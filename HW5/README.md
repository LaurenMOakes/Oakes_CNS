1/c Lauren Oakes 

Computer and Network Security 

04 Oct 2023

# Redhat Academy Screenshots
10.2 #6 - This command shows that a root user is already logged in the server we SSHed into, we will use this info to SSH into the same server using this 
identified root user.

10.2 #12 - This command will SSHT into server b as the student user but use hostname argument to prevent access through the interactive shell.

10.4 #4 - This command sends public key information to operator1 on server a, then SSHEed into server a using those credentials. Shows successful SSH, but 
unsuccessful check of SSH keys.

10.4 #9 - This command tests SSHing into operator1 on server a again but using key2 this time which uses passphrases for another level of security as seen below.

# Applying Key Based Authentication 
This command generates a shared public key to authenticate SSH login attempts. 

This command copies generated key to jumpbox using the SCP command.

This command SSHes into jumpbox and shows location and existence of key in the jumpbox.


# Brute Forcing Passwords
Disclaimer - I had to download Ubuntu Linux using WSL on my NUC in order to install and run Hydra. 
This command used a specified username (Oakes) and a list of passwords (as specified) to attack the jumpbox through SSH. Shows succesful brute force attack.
