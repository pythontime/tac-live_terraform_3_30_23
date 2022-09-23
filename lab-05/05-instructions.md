# Lab 05 - AWS Config with SSH and Outputs
Here you will build on Lab 04 by adding proper SSH support. You'll also learn how to use outputs to have Terraform tell you information you need to know, such as the IP address and name of an instance.
Finally, we'll use cloud-init to provide additional configuration details to our build.

# Procedure
This lab is a bit more in-depth, so go slow, and take it step-by-step. This time we'll be using a current Ubuntu image. If you get stuck, view the solution in the /solution directory. 

## Create a directory structure
Create three new directories: instances, keys, and scripts.
For example: `mkdir {instances,keys,scripts}`
- Your main.tf file will go into the instances directory. This is the directory where you will run your Terraform commands.
- Your SSH keys will be placed in the keys directory.
- Your cloud-init script (provided) will go in the scripts directory.

## Create an SSH key pair
You will need openssh or another SSH tool installed. 
- Run the command `ssh-keygen` to create an SSH key pair.

> NOTE: Consider using ED25519 instead of the default RSA. 
> For example: `ssh-keygen -t ed25519`

- Name the key "aws_key" and save the key to the "keys" directory.

> NOTE: The solution has a key pair, but the private key has been compromised (for the very fact that it exists and you can see it.) Do not use that key! Delete it and create a new one!




