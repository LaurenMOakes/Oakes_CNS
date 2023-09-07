1/c Lauren Oakes 

Computer and Network Security 

07 Sep 2023

# Tutorial 1 & 2

I used virtual studio in order to create my bootstrap file and had no problem using the vagrant ssh command to gain access 
to my virtual machine, however when I ran the command that was meant to print my html file, nothing would print to screen.
Screenshots are below to showcase my problems and end result. 

Lab html directory including neccesary files - Vagrantfile, bootstrap.sh, and Homework_1.html

![](https://github.com/LaurenMOakes/Oakes_CNS/blob/main/HW1/files.png?raw=true)

Running vagrant ssh and wget -qO- 10.0.2.15

![](https://github.com/LaurenMOakes/Oakes_CNS/blob/main/HW1/vagrant_ssh.png?raw=true)

Bootstrap.sh file to show Vagrant configurations

![](https://github.com/LaurenMOakes/Oakes_CNS/blob/main/HW1/bootstrap.png?raw=true)

# Vagrant Provisoner - Puppet Salt

Allows for use of Puppet which is a software configuration management tool that basically automates server configuration
with little coding needed.

To use this provisioner you must allow it via config.vm.provision "puppet" and other configuration updates in the Vagrantfile as well as install puppet. 

on the guest machine that you will be working with. 
