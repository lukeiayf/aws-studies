- File Storage
	- Tree like structure, the most common in OS organization
- Block Storage
	- Split files into fixed-sized chunks of data called blocks, each with its own address
	- Optimized for low-latency operations, high performance (transactions, containers, VMs)
- Object Storage
	- Treats each file as an object, a distinct single unit of data 
	- General data storage or large &/or unstructured data sets(archives, backups, multimedia)
### **Block Storage**

**What it is:**  
Block storage divides data into fixed-size blocks and stores them separately, each with a unique address. The operating system manages these blocks, which can be assembled into files as needed.

**How it works in AWS:**

- Provided by **Amazon EBS (Elastic Block Store)**
- Volumes are attached to EC2 instances as virtual hard drives
- Acts like a traditional disk drive; you can format, partition, and manage it as you would a physical disk

**Use cases:**

- Databases (e.g., MySQL, Oracle)
- Applications requiring low-latency, high-performance storage
- Boot volumes for EC2 instances

---

### **File Storage**

**What it is:**  
File storage organizes data as files in directories and subdirectories, similar to how files are stored on your computer. It uses standard file system protocols (like NFS or SMB).

**How it works in AWS:**

- Provided by **Amazon EFS (Elastic File System)** and **Amazon FSx**
- Multiple EC2 instances can access the same file system at the same time
- Supports shared access and file-level permissions

**Use cases:**

- Shared storage for web servers or content management systems
- Home directories for users
- Lift-and-shift of on-premises file-based applications

---

### **Object Storage**

**What it is:**  
Object storage manages data as objects, each containing the data itself, metadata, and a unique identifier. There’s no hierarchy (like folders); everything is stored in a flat address space.

**How it works in AWS:**

- Provided by **Amazon S3 (Simple Storage Service)**
- Objects are stored in “buckets”
- Designed for massive scalability and durability

**Use cases:**

- Storing backups, media files, and big data
- Data lakes and analytics
- Static website hosting
- Archival and compliance storage (with S3 Glacier)

---

**Summary:**

- **Block storage** (EBS): Like a hard drive, for databases and OS disks
- **File storage** (EFS, FSx): Like a shared network drive, for shared file access
- **Object storage** (S3): For scalable, durable storage of files and data as objects, ideal for backups, media, and big data