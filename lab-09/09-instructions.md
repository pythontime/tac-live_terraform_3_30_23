# Lab 09 - Working with Terraform Cloud (TC)
In this lab we'll:
- Create a Terraform Cloud account
- Create a workspace
- Complete a Terraform run using the CLI

## Create a TC account
https://app.terraform.io

You will need a valid email address to validate your account.

> Note: You will also need to use a strong password. Might I suggest KeePass as your password vault: https://keepass.info/download.html

> Note: You can also go to the Hashicorp Cloud Portal: https://app.terraform.io/public/signup/account?product_intent=terraform&utm_source=learn

## Configure TC
- Create a new organization name (it must be unique!)
- Select CLI-driven workflow
- Name and describe your first workspace

## Configure the main.tf file
- Copy the example code from the overview webpage to the main.tf file.
- run `terraform init` and notice how it fails.
  
## Login to TC with a token
- Use the `terraform login` command.
- Copy and paste the token from the browser to the CLI.
- Verify that the connection is valid.

> Note: take a look at the .terraform.d directory and locate the credentials.tfrc.json file. This contains your Terraform Cloud token.

## Setup a new AWS access key
- Create a new access key in the AWS console
- Copy the access key ID and secret key to cred.tf

## Initialize and apply the code
- Type `terraform init` and verify that the directory was initialized properly.
- Type `terraform apply` 
- Verify that the instance was created in the AWS console
- Check the run in the Terraform Cloud
- Compare the local state file with the remote state file

## Destroy and logout
- Type `terraform destroy` to destroy the AWS infrastructure.
- Use the `terraform logout` command to end the cloud session and delete the token
  
> Note: Analyze the .terraform.d directory again - the token should be gone.

---
## *Another job well done!*
---


