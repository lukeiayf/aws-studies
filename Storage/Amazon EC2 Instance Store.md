
- **Definition:**  
	An instance store provides ephemeral block-level storage(see [[Storage Types]]) for the [[EC2 instance]]. 
	
    An EC2 instance store provides block-level storage that is physically attached to the host server running your EC2 instance. It is sometimes called “ephemeral storage” because the data does not persist after the instance stops, terminates, or fails.
    
- **How it works:**  
    When you launch an EC2 instance with instance store volumes, the storage is available for use as soon as the instance starts. You can use it for temporary files, caches, buffers, or any data that can be recreated or is not critical.
    
- **Persistence:**  
    Data in an instance store is **lost** if:
    - The instance is stopped or terminated
    - The underlying hardware fails
    
- **Comparison to EBS:**  
    Unlike **Amazon EBS** (see [[EBS Volume]]), which is network-attached and persists independently of the instance lifecycle, instance store volumes are tied to the life of the instance.