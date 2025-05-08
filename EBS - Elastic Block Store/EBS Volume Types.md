	 
- See [[EBS Volume]]

 - **SSD-backed volumes** include General Purpose SSD (`gp3`, `gp2`) for balanced price and performance, and Provisioned IOPS SSD (`io2`, `io1`) for high-performance, I/O-intensive workloads like large databases.

- gp2/3 are used for effective storage and low latency
- io1/2 are used for database workloads

- Only io1/2 are available for multi attach and specified into one AZ. And a multi attach can be attached to up to 16 [[EC2]] instances at a time

- **HDD-backed volumes** include Throughput Optimized HDD (`st1`) for high-throughput, frequently accessed workloads like big data and log processing, and Cold HDD (`sc1`) for infrequently accessed, archival storage at the lowest cost.


- **Only gp2/3 and io1/2 can be used as boot volumes**
