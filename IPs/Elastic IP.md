- When you stop and then start an [[EC2]] instance it can change its public IP
- If you need to have a fixed public IP for the instance an Elastic IP is needed
- An elastic IP is a public IPV4 IP you own as long as you don't delete it
- You can attach it to one instance at a time
- You can mask the failure of an instance by quickly remapping the address to another instance.
- You can only have 5 EIP

**TRY TO AVOID USING EIP INSTEAD USE RANDOM PUBLIC IPS AND REGISTER A DNS NAME TO IT(SEE [[Route 53]] or use [[ELB - Elastic Load Balancer]])**
