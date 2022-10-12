# Lab 06 - Working with Variables
Here you will define elements of your configuration using variables instead of hard-coding them into the main terraform file.

## Procedure
- Open the lab-06 directory. (This will be your working directory.)
- Analyze the main.tf file. This is essentially the same file we used in Lab 04. 
- Create a new file called variables.tf. Copy the code from code-variables.txt to variables.tf. Analyze that new code.
- Modify the main.tf file. Find the "Name" tag. Modify it so that it calls the variable. For example:
  `Name = var.instance_name`
  