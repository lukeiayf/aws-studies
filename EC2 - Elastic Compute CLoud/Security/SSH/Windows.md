Before being able to SSH into an EC2 instance it is necessary to have access to the .pem file generated when creating the instance. You must run the commands in the directory the file is located using powershell or cmd.

The command to ssh is:
`ssh -i [.pem file] ec2-user@[EC2 instance ipv4 address]`

If the terminal gives unprotected file error, you must change the permissions of the file, a good example is to just let the user be able to access it. File -> properties -> security

To exit the instance in ssh type exit