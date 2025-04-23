See [[Storage Types]] for what is a file storage

See [[EFS – Elastic File System]]

**Amazon EFS (Elastic File System)** is a fully managed, scalable, elastic, cloud-native NFS (Network File System) file storage service for use with AWS Cloud services and on-premises resources.

Here's a breakdown:

- **Fully Managed:** AWS handles the setup, patching, backup, and maintenance.
- **Scalable and Elastic:** Automatically grows and shrinks as you add or remove files, so you only pay for the storage you use.
- **NFS File System:** Uses the standard NFS protocol, making it compatible with Linux-based workloads.
- **Shared File Storage:** Multiple EC2 instances can access the same EFS file system concurrently.
- **Cloud-Native:** Designed to integrate seamlessly with other AWS services.
- **On-premises Access:** Can be accessed from on-premises servers via AWS Direct Connect or VPN.

**In simpler terms:**

Think of Amazon EFS as a network drive in the cloud that can be accessed by multiple computers ([[EC2 instance]]) at the same time. It automatically scales its storage capacity as needed, and you don't have to worry about managing the underlying infrastructure.

**Key Use Cases:**

- Web serving and content management
- Application development and testing
- Media and entertainment workflows
- Big data analytics
- Machine learning
- Container storage
- Backup and disaster recovery
