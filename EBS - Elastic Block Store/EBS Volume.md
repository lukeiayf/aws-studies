• An EBS (Elastic Block Store) Volume is a network drive you can attach
to your [[EC2 instance]] while they run
• It allows your instances to persist data, even after their termination
• They can only be mounted to one instance at a time (at the Certified Cloud Practitioner - CCP level)
• They are bound to a specific availability zone
• Analogy: Think of them as a “network USB stick”
• It’s a network drive (i.e. not a physical drive)
• It uses the network to communicate the instance, which means there might be a bit of
latency
• It can be detached from an EC2 instance and attached to another one quickly
• It’s locked to an Availability Zone (AZ)
• An EBS Volume in us-east-1a cannot be attached to us-east-1b
• To move a volume across, you first need to create an [[EBS Snapshot]] of it
• Have a provisioned capacity (size in GBs, and IOPS)
• You get billed for all the provisioned capacity
• You can increase the capacity of the drive over time