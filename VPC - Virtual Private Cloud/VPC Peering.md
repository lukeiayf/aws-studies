• Connect two VPC, privately using AWS’ network
• Make them behave as if they were in the same network
• Must not have overlapping CIDR (IP address range)
• VPC Peering connection is not transitive (must be established for
each VPC that need to communicate with one another)