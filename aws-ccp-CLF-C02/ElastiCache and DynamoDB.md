## ElastiCache
This is a web service with in-memory data store - faster read/write will happen since queries made are cached and will not read/write to the actual DB itself. Given this caching setup, this reduces load off of databases with high workloads

## DynamoDB
It's a **NoSQL DB**. Even though we store items (together with its attribute/s) in tables, there is no relationship a.k.a *nonrelational* among tables created. I'd like to think of it as a *flat table*; there is no normalization and all columns for each record are stored in one table only.

It's also a "serverless" DB. We just create tables in the cloud without having to think of any compute.

Performance wise, it scales based on high workload with low latency retrieval

The type of data of data it uses is **key-value**. One good example is JSON. There's actually an option for us to view stored items in DynamoDB using vanilla JSON and "DynamoDB JSON" version.

## DynamoDB Global Tables
These feature allows table access with *low latency* in multiple regions. We can read/write to any region using **Active-Active** replication  (2-way replication from both regions).


---
**Tags:** #aws #cloud #database #dynamoDB #nosql #elasticache

