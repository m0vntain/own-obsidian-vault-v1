
# High Level

AWS offers two ways to create Relational DB:
1. RDS (Relational Database Service)
2. Amazon Aurora

Both services have different features to support for high availability and usual failovers which a database service normally could encounter.

# Notes

### RDS
- create relational DB using different engines in AWS (Oracle, MySQL, Postgres, etc.) - 8 total engines
- **snapshots**:
	- restore - create new DB from existing snapshot
	- copy - restore DB to another region
	- share - other to use snapshot to create DB
- deployment options:
	- **read replicas**
		- *scale out* DB instances to handle more workload (15 replicas)
		- writes only to the the *main RDS*
	- **Multi-AZ**
		- provides *high availability*
		- support for *failovers*
		- RDS - automatically provisions and maintains a synchronous standby replica in a different AZs
		- primary DB - synchronously replicated across AZs to a standby replica


### Amazon Aurora Serverless option
- Did not delve deep into this service (at least of CCP certification) but it can basically increase throughput of MySQL and Postgres by x5
- part of Amazon RDS
- full managed relational DB
- proxy fleet
- use cases

---
**Resources**:
- [What is Amazon Relational Database Service (Amazon RDS)? - Amazon Relational Database Service](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html)
- [What is Amazon Aurora? - Amazon Aurora](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html)
- [Multi-AZ DB instance deployments - Amazon Relational Database Service](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.MultiAZSingleStandby.html)


---
**Tags:** #aws #cloud #rds #database #aurora
