**Azure SQL Server vs Azure SQL DB**
- Azure SQL server allows to perform multiple administrative tasks (i.e. control logins, firewall rules, security policies, failower groups, auditing etc).

**Azure SQL pricing models**
- vCores:
- 1 vCore=1 logical CPU

- You can choose computer and storage independently

- 2 models:
*Provisioned* - you need to specify exact amount of compute resources that are always provisioned for you (v/core unit price is lower in provisioned mode)
*Serverless* - you need to specify range of computer resources which are provisioned based on usage
- 3 tiers:
-- *General purpose*- most business workloads, balance between performance and costs.
-- *Business critical* - adds higher resilience to failures and I/O performance.
-- *Hyperscale* - business workloads that requires highly scalable storage and reads operations.

**vCores - service tiers**
- Different service tiers offer different limits: Storage/Iops and throughput/Availability/Backup

**vCores - which tier to choose?**
1.  *General purpose*- most often used, 99.99% SLA
2.  *Business critical*- Low IO latency, a lot of updates, long running transactions, when you need higher SLA (99.995%), fast backup recovery etc.
3.  *Hyperscale* - when you have large database (up to 100 TB), or moving large DB from on-prem to the cloud, or when you need fast scaling.

**vCores - serverless**
Automatically scales the DB based on workload, automatically pauses the DB when there are no queries (no vCores cost). You can define MIN, MAX vCores, define autopause delay.
*Available for General purpose tier only!*

**When to use Serverless?**
- DB with unpredictable activity and significant idle time, frequent scaling workload, when warm-up latency is expected.

**vCores pricing**
Total price = vCore price + data storage price.



