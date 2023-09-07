1/c Lauren Oakes
- Computer and Network Security 
- 07 SEP 2023

# **Container Summaries**

## Node
Node is another docker image I spent some time looking into, and although this image contains much more documentation I decided not to use this image 
because there was no direct tests that I found to run on the container. However, this image serves as a platform for software running networking applications
in order to assist in scalability. What is unique about this container is it offered multiple different versions for differant scalability goals.

## GCC
GCC is part of the GNU Compiler Collection by the GNU Project that serves as a compiler for multiple coding languages and is labeled a vital component of the
GNU toolchain. This container took much more prerequisets to use because it required the input of a coding application in order to use the compiler function
of the container.

# **Container I Used**

## Cowrie
Cowrie was a suggested docker image that does not include much documentation but serves a purpose of logging attackers brute force and shell interactions. 
The one helpful peice of documentation for this iamge was a description of how to test image by running ssh on the designated port. I ended up using this
image because of its simplicity, I had a hard time figuring out how to properly integrate more advanced or complicated images.

# Errors

While completing this lab I encountered many errors while trying to build my new docker-compose.yml file. At first it was just simple yml text errors that 
I was able to troubleshoot but eventually the errors became about my defining objects within the code file and I was not able to figure this out. I used my 
docker-compose file from Lab 2 and added a new host under my new Cowrie docker image except the integration within the network subsection in the new yml 
file was not configured correctly and I could not find a solution that still alowed my new host to be connected to the same network as my last host. Images
of the error can be seen in the HW2 folder of this repository.
