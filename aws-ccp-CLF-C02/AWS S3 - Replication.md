**Tags**: #aws #s3 #cloud

**Resources:**
- [AWS S3 Docs - Replication](https://docs.aws.amazon.com/AmazonS3/latest/userguide/replication.html)
## Overview
- used to copy objects between S3 buckets
- *asynchronous* copying/replication
- can replicate to **single** or **multiple** destination buckets

## Types of *Live* Replication
1. Cross-Region Replication (CRR)
	- replicate buckets in ***different* AWS regions**
2. Single-Region Replication (SRR)
	- replicate buckets in ***same* AWS regions** 

> [!Note]
> When creating buckets with replication, make sure to set the **Bucket Versioning** to  `Enabled`. Replication only works if versioning is enabled for the buckets (origin & destination). 
