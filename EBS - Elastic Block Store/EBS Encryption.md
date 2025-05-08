-  Encrypting an [[EBS Volume]] provides encrypt for:
	- Data at rest inside the volume
	- Data in transit between the [[EC2]] instance and the EBS Volume
	- All the [[EBS Snapshot]]
	- All volumes created from the snapshot

- Encryption is recomended as it has minimal impact on latency
- Leverages keys from [[KMS - Key Management Service]]