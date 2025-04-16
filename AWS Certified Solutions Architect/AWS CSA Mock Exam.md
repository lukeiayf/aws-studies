#### **Question 1: Scenario-Based**

A company is running a web application on Amazon EC2 instances behind an Elastic Load Balancer (ELB). The application stores user-uploaded files in an Amazon S3 bucket. The company wants to ensure that the files are encrypted at rest and that only the application can access the bucket. What should the company do to meet these requirements?

**Options:** a) Enable server-side encryption on the S3 bucket and create a bucket policy that allows access only from the ELB.  
b) Enable server-side encryption on the S3 bucket and create a bucket policy that allows access only from the EC2 instances.  
c) Enable client-side encryption on the application and store the encryption keys in the EC2 instance.  
d) Enable server-side encryption on the S3 bucket and use an IAM role attached to the EC2 instances to access the bucket.

###### **Answer:**
**d)** Enable server-side encryption on the S3 bucket and use an IAM role attached to the EC2 instances to access the bucket.  
**Explanation:** Server-side encryption ensures that the files are encrypted at rest. Using an IAM role attached to the EC2 instances allows secure access to the S3 bucket without hardcoding credentials.

---

#### **Question 2: Multiple-Choice**

Which AWS service can be used to improve the performance of a read-heavy application by caching frequently accessed data?

**Options:** a) Amazon RDS  
b) Amazon DynamoDB Accelerator (DAX)  
c) Amazon ElastiCache  
d) Amazon CloudFront

###### **Answer:**  
**b)** Amazon DynamoDB Accelerator (DAX)  
**c)** Amazon ElastiCache  
**Explanation:** DAX is a caching layer for DynamoDB, while ElastiCache provides in-memory caching for other databases or applications. Both improve read performance.

---

#### **Question 3: Scenario-Based**

A company is designing a disaster recovery solution for its critical application hosted in AWS. The application uses an Amazon RDS database and stores files in an S3 bucket. The company wants to ensure that the application can failover to another AWS region with minimal downtime. What should the company do?

**Options:** a) Enable Multi-AZ for the RDS database and replicate the S3 bucket to another region using Cross-Region Replication.  
b) Enable Multi-AZ for the RDS database and use S3 Transfer Acceleration for faster uploads.  
c) Create a read replica of the RDS database in another region and enable S3 Cross-Region Replication.  
d) Create a read replica of the RDS database in another region and use S3 lifecycle policies to move data to Glacier.

###### **Answer:**  
**c)** Create a read replica of the RDS database in another region and enable S3 Cross-Region Replication.  
**Explanation:** Multi-AZ is for high availability within a single region, not disaster recovery. A read replica in another region ensures the database is available in case of a regional failure, and S3 Cross-Region Replication ensures the files are replicated to another region.

---

#### **Question 4: True/False**

AWS Trusted Advisor can provide recommendations for cost optimization, security, fault tolerance, and performance.

###### **Answer:**  
**True**  
**Explanation:** AWS Trusted Advisor provides insights and recommendations across multiple categories, including cost optimization, security, fault tolerance, performance, and service limits.

---

#### **Question 5: Multiple-Response**

Which of the following are valid ways to reduce costs in AWS? (Select TWO)

**Options:** a) Use Spot Instances for non-critical workloads.  
b) Use Multi-AZ deployments for all resources.  
c) Use S3 Intelligent-Tiering for infrequently accessed data.  
d) Use On-Demand Instances for predictable workloads.  
e) Use Amazon CloudFront for all data transfers.

###### **Answer:**  
**a)** Use Spot Instances for non-critical workloads.  
**c)** Use S3 Intelligent-Tiering for infrequently accessed data.  
**Explanation:** Spot Instances are cost-effective for non-critical workloads, and S3 Intelligent-Tiering automatically moves data to lower-cost storage tiers based on access patterns.

---

#### **Question 6: Scenario-Based**

A company is hosting a global application that serves users from multiple continents. The application uses an Amazon S3 bucket to store static content. Users are reporting high latency when accessing the content. What should the company do to reduce latency?

**Options:** a) Enable S3 Transfer Acceleration.  
b) Use Amazon CloudFront to cache the content at edge locations.  
c) Enable Cross-Region Replication for the S3 bucket.  
d) Use AWS Global Accelerator to route traffic to the S3 bucket.

###### **Answer:**  
**b)** Use Amazon CloudFront to cache the content at edge locations.  
**Explanation:** CloudFront caches content at edge locations closer to users, reducing latency. S3 Transfer Acceleration improves upload speeds but does not cache content.

---

#### **Question 7: Fill-in-the-Blank**

Amazon ________ is a fully managed NoSQL database service that provides single-digit millisecond latency at any scale.

###### **Answer:**  
**DynamoDB**  
**Explanation:** Amazon DynamoDB is a NoSQL database service designed for high performance and scalability.

---

#### **Question 8: Scenario-Based**

A company wants to monitor its AWS environment for unauthorized changes to its resources. Which AWS service should they use?

**Options:** a) Amazon CloudWatch  
b) AWS Config  
c) AWS CloudTrail  
d) Amazon GuardDuty

###### **Answer:**  
**c)** AWS CloudTrail  
**Explanation:** AWS CloudTrail logs all API activity in the account, allowing the company to monitor and audit changes to resources.

---

#### **Question 9: Multiple-Choice**

Which AWS service is best suited for running containerized applications without managing the underlying infrastructure?

**Options:** a) Amazon ECS  
b) Amazon EKS  
c) AWS Fargate  
d) AWS Lambda

###### **Answer:**  
**c)** AWS Fargate  
**Explanation:** AWS Fargate is a serverless compute engine for containers, allowing you to run containerized applications without managing servers.

---

#### **Question 10: Scenario-Based**

A company is running a high-performance computing (HPC) workload that requires a shared file system with low latency. Which AWS service should they use?

**Options:** a) Amazon S3  
b) Amazon EFS  
c) Amazon FSx for Lustre  
d) Amazon RDS

###### **Answer:**  
**c)** Amazon FSx for Lustre  
**Explanation:** FSx for Lustre is designed for HPC workloads requiring a high-performance, low-latency file system.

---
