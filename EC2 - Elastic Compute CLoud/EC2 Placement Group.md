The strategy to to control EC2 instances placement can be defined using placement groups.
"They provide control over how instances are physically located within AWS data centers."

**PARTITION = HARDWARE RACK**

- Cluster - clusters instances into low-latency groups in a single AZ, placed in close proximity
- Spread - spreads instances across underlying hardware, spread far apart
- Partition - spreads instances across many different partitions whitin an AZ. Scales to the hundreds
