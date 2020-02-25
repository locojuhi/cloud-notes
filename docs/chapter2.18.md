# Databases

## Relation database (RDS)
- SQL Server
- Oracle
- Mysql Server
- PostgreSQL
- Aurora
- MariaDB

### Features of RDS
- Multi-AZ - For disaster recovery (fail over)
- Read Replicas - For perfomance

## No Relational database
- DynamoDB

## OLTP vs OLAP
### Online Transaction Processing (OLTP)
Specific record, somethign small and specific.

### Online Analitycs Processing (OLAP)
A lot a mount of data, or expexive processing for the database

#### Datawarehousing
Used for business intelligence. Tools like cognos, jaspersoft, SQL Server Reporting Services, Oracle hyperion, sap netwaver.
Used to pull in very large and complet data sets. Usually used by management to do queries on data (such as current perfomance vs targets).
Redshift

## Elastic cache
Is a service that makes it easy to deploy, operate and scale an in-memory cache in the cloud.

### Engines:
- Memcached
- Redis

## Examp tips
- RDS(SQL/OLTP)
    - SQL
    - MySQL
    - PostgreSQL
    - Oracle
    - Aurora
    - MariaDB
- DynamoDB(No SQL)
- RedShift(OLAP) -> analitycs, complex queries
- Elasticache
    - Memcached
    - Redis
- Redshift for BI or datawarehousing    

## Exam tips
- Multi AZ for disaster recovery
- Read replica - for perfomance
