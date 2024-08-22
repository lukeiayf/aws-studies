• Aurora is a proprietary technology from AWS (not open sourced)
• PostgreSQL and MySQL are both supported as Aurora DB
• Aurora is “AWS cloud optimized” and claims 5x performance improvement over MySQL on RDS, over 3x the performance of Postgres on RDS
• Aurora storage automatically grows in increments of 10GB, up to 128 TB
• Aurora costs more than RDS (20% more) – but is more efficient
• Not in the free tier
• Automated database instantiation and auto-scaling based on actual usage
• PostgreSQL and MySQL are both supported as Aurora Serverless DB
• No capacity planning needed
• Least management overhead
• Pay per second, can be more cost- effective
• Use cases: good for infrequent,intermittent or unpredictable workloads…

**Read Replicas:**

• Scale the read workload of your DB
• Can create up to 15 Read Replicas
• Data is only written to the main DB

**Multi-AZ**:

• Failover in case of AZ outage (high availability)
• Data is only read/written to the main database
• Can only have 1 other AZ as failover