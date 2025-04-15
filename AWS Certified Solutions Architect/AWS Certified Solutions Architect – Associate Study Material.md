
### **Domain 1: Design Secure Architectures (30%)**

#### **1.1 Secure Access to AWS Resources**

- **Key Services**: IAM, AWS Organizations, AWS SSO, Security Groups, NACLs
- **Best Practices**:
    - Implement the principle of least privilege.
    - Use IAM roles for applications instead of hardcoding credentials.
    - Enable MFA for all users, especially root accounts.
    - Use AWS Organizations and Service Control Policies (SCPs) for account governance.
- **Example**:
    - A company uses IAM roles for EC2 instances to access S3 buckets securely. Security Groups allow only HTTPS traffic, and NACLs block unauthorized IP ranges.

#### **1.2 Data Encryption**

- **Key Services**: AWS KMS, AWS CloudHSM, S3 Encryption, ACM
- **Best Practices**:
    - Encrypt data at rest using KMS-managed keys.
    - Use TLS for encrypting data in transit.
    - Rotate encryption keys regularly.
- **Example**:
    - A healthcare app encrypts patient data in S3 using KMS and ensures all API calls use HTTPS with ACM-managed certificates.

#### **1.3 Security Controls**

- **Key Services**: AWS WAF, Amazon GuardDuty, AWS Config, AWS Shield
- **Best Practices**:
    - Use WAF to block malicious traffic.
    - Enable GuardDuty to detect threats.
    - Use AWS Config to monitor compliance.
- **Example**:
    - A financial app uses WAF to block SQL injection attacks and GuardDuty to monitor unusual activity.

---

### **Domain 2: Design Resilient Architectures (26%)**

#### **2.1 Scalability**

- **Key Services**: Auto Scaling, Elastic Load Balancer (ELB), Amazon CloudWatch
- **Best Practices**:
    - Use Auto Scaling to handle traffic spikes.
    - Distribute traffic with ELB.
    - Monitor performance with CloudWatch.
- **Example**:
    - An e-commerce site uses Auto Scaling to add EC2 instances during sales events and ELB to distribute traffic.

#### **2.2 Fault Tolerance**

- **Key Services**: Multi-AZ Deployments, S3, DynamoDB
- **Best Practices**:
    - Deploy resources across multiple AZs.
    - Use stateless applications with S3 or DynamoDB for state storage.
- **Example**:
    - A web app deploys EC2 instances in multiple AZs with ELB. If one AZ fails, traffic is routed to healthy instances.

#### **2.3 High Availability**

- **Key Services**: Amazon RDS Multi-AZ, Route 53
- **Best Practices**:
    - Use Multi-AZ for databases.
    - Use Route 53 for DNS failover.
- **Example**:
    - A database uses RDS Multi-AZ for automatic failover, and Route 53 redirects traffic to a backup region during outages.

#### **2.4 Disaster Recovery**

- **Key Services**: S3 Cross-Region Replication, AWS Backup, Route 53
- **Best Practices**:
    - Use S3 for backups and Glacier for archival.
    - Implement cross-region replication for critical data.
- **Example**:
    - A critical app replicates S3 data to another region and uses Route 53 to redirect traffic during disasters.

---

### **Domain 3: Design High-Performing Architectures (24%)**

#### **3.1 Compute Optimization**

- **Key Services**: EC2, AWS Lambda, ECS, EKS
- **Best Practices**:
    - Use Spot Instances for cost savings.
    - Use Lambda for event-driven workloads.
    - Use ECS or EKS for containerized applications.
- **Example**:
    - A video processing app uses Lambda for transcoding and Spot Instances for batch processing.

#### **3.2 Storage Optimization**

- **Key Services**: S3 Intelligent-Tiering, EBS, FSx
- **Best Practices**:
    - Use S3 Intelligent-Tiering for cost savings.
    - Use EBS Provisioned IOPS for high-performance workloads.
- **Example**:
    - A data analytics app stores raw data in S3 and uses FSx for Lustre for processing.

#### **3.3 Database Optimization**

- **Key Services**: RDS, DynamoDB, Redshift
- **Best Practices**:
    - Use RDS read replicas for scaling.
    - Use DynamoDB Accelerator (DAX) for caching.
- **Example**:
    - An e-commerce app uses RDS for transactions and DynamoDB for session management.

#### **3.4 Network Optimization**

- **Key Services**: CloudFront, VPC, Global Accelerator
- **Best Practices**:
    - Use CloudFront for content delivery.
    - Use VPC endpoints to reduce data transfer costs.
- **Example**:
    - A global SaaS app uses CloudFront for static content and Global Accelerator for dynamic content.

---

### **Domain 4: Design Cost-Optimized Architectures (20%)**

#### **4.1 Cost-Effective Compute**

- **Key Services**: Spot Instances, Savings Plans, Auto Scaling
- **Best Practices**:
    - Use Spot Instances for non-critical workloads.
    - Use Savings Plans for predictable workloads.
- **Example**:
    - A batch processing app uses Spot Instances to save up to 90% on compute costs.

#### **4.2 Cost-Effective Storage**

- **Key Services**: S3 Glacier, EBS Snapshots, Lifecycle Policies
- **Best Practices**:
    - Use Glacier for archival.
    - Automate data movement with lifecycle policies.
- **Example**:
    - A media company uses S3 Glacier for archiving old videos and lifecycle policies to move infrequently accessed data.

#### **4.3 Cost-Effective Networking**

- **Key Services**: CloudFront, VPC Endpoints, Direct Connect
- **Best Practices**:
    - Use CloudFront to reduce data transfer costs.
    - Use VPC endpoints to avoid public internet traffic.
- **Example**:
    - A global app uses CloudFront for caching and VPC endpoints for secure, cost-effective access to S3.

---

### **Practice Questions**

1. **Scenario-Based Question**:  
    A company wants to host a web application with high availability and fault tolerance. The application should handle traffic spikes during sales events. Which AWS services should they use?
    - **Answer**: EC2 Auto Scaling, Elastic Load Balancer, RDS Multi-AZ, Route 53.
2. **Multiple-Choice Question**:  
    Which AWS service is best for storing infrequently accessed data at the lowest cost?
    - **Options**:  
        a) S3 Standard  
        b) S3 Intelligent-Tiering  
        c) S3 Glacier  
        d) EBS
    - **Answer**: c) S3 Glacier.

---

### **Additional Resources**

- **AWS Well-Architected Framework**: [AWS Well-Architected](https://aws.amazon.com/architecture/well-architected/)
- **AWS Training**: [AWS Skill Builder](https://aws.amazon.com/training/)
- **AWS Whitepapers**: [AWS Whitepapers](https://aws.amazon.com/whitepapers/)