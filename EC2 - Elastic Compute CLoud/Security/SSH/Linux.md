Before being able to SSH into an EC2 instance it is necessary to have access to the .pem file generated when creating the instance. You must run the commands in the directory the file is located.

The command to ssh is:
`ssh -i [.pem file] ec2-user@[EC2 instance ipv4 address]`

If the terminal gives unprotected file error, you must change the permissions of the file first a good one is, which means only the user can read the file:
`chmod 0400 [.pem file] `

To exit the instance in ssh type exit or ctrl+g