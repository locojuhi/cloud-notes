# Architecting for the cloud best practices - Part 2
## Databases
### Relational Databases (Aurora)
- Scalability
- Hihg availability - Multi AZ
- Anti patterns - no need for joins or complex transactions, use NO-SQL

### Non-Relational database (DynamoDB)
- Scalability
- Hihg availability - Multi AZ
- Anti patterns - requires joins or complex transactions. use relational datbase (Aurora or others). If you have large binary files (audio, video and image consider storing the files in Amazon S3)

### Data warehouse (Redshift)
- Scalability
- High Availability - Multi AZ
- Anti patterns - Not meant for on line transcation processin (OLTP)

### Search - ElasticSeach
- Scalability
- High availavility

### Graph Database Amazon Neptune
- Scalability
- High Availability

### Manage Incresing Volumes of Data
A data lake is an architectureal approach that allows you to store massive amounts of data  in a central location so that it's readily available to categorized, processed, analyzed and consumed by diverse groups within your organization

### Removing single points of failure
 - Introducing Redundancy
 - Detect Failure
 - Durable Data Storage
 - Automated multi data centre resilience
 - Fault isolation and tradicional horizontal scaling
 - Sharding

### Optimize for cost
- Right Sizing
- Elasticity
- Take advantage of the variety of purchasing options
    - Spot Instances
    - Reserved Capacity

### Caching
- Application caching
- Edge caching

### Security
- Use AWS Features for defense in depth
- Share security resposability with AWS
- Reduce privileged Access
- Security as code
- Real time auditing

# Read the paper
https://d1.awsstatic.com/whitepapers/AWS_Cloud_Best_Practices.pdf