# AWS Pricing
Capex vs Opex

## Capex
Stands for capital Expenditure which where you pay up front. It's a fixed, sunk cost

## Opex
Stands for operation expenditure which is where you pay for what you use.

## Pricing policies
- Pay as you go
- Pay less when you reserve
- Pay even less per unit by using more
- Pay even less as aws grows
- Custom pricing

## Key principles and best practices
- Understand the fundamentals of pricing
- Start early with cost optimization
- Maximize the power of flexibility
- Use the right pricing model for the job

### Driver cost
- Compute
- Storage
- Data outbound

### Use the right pricing model for the job
- On demand
- Dedicated Instances
- spot Instances
- Reservation

### Free services
- VPC
- Elastic Beanstalk
- CloudFormation
- Identity Access Management (IAM)
- AutoScaling
- Opsworks
- Consolidated billing

### EC2 Pricing
#### What determines price?
- Clocks hours of server time
- Instance type
- Pricing model
    - reserved
    - spot
    - on demand
- Number of instances
- Load balancing
    - Application LB
    - Classic LB
    - Network LB
- Detailed monitoring
- AutoScaling
- Elastic ip Addresses
- Operating systems and software packages
    - Windows for example

### Lambda Pricing
#### What determines price?
- Request Pricing
    - Free Tier: 1 milliion request per month
    - 0.20 per 1 million request thereafter
- Duration pricing
    - 400000 GB-Seconds per month free, up to 3.2 million seconds of compute time
    - 0.00001667 for every GB-second used thereafter
- Additional charges
    - You may incur additional charges if your lambda function uses other aws services or transfer data. For example, if your lambda function reads and writes data or from S3. You will be billed for the read/write request and the data stored in S3

### EBS Pricing
#### What determines price?
- Volumes (per GB)
- Snapshots (per GB)
- Data transfer

### S3 Pricing
#### What determines price?
- Storage classes
- Storage
- Request (GET, PUT, COPY)
- Data transfer

### Glacier Pricing
#### What determines price?
- Storage
- Data retrieval times

### Snowball Pricing
#### What determines price?
- Service fee per job
    - Snowball 50 TB: 200
    - Snowball 80 TB: 250
- Daily Charge
    - First 10 days are free, after that it's a 15 a day
- Data transfer
    - Data transfer in to S3 is free. Data transfer out is not. 

### RDS Pricing
#### What determines price?
- Clock hours server time
- DB characteristics
- purchase type
- Number of database instances
- Provisioned storage
- Requests
- Deployment type
- Data transfer

### DynamoDB Pricing
#### What determines price?
- Provisioned throughput (write)
- Provisioned throughput (read)
- Indexed data storage

### Cloudfront Pricing
#### What determines price?
- Traffic Distributtion
- Requests
- Data Transfer Out

Read this thow whitepapers:
- https://d1.awsstatic.com/whitepapers/AWS_Cloud_Best_Practices.pdf
- https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf
- https://aws.amazon.com/cloudformation/
- https://aws.amazon.com/es/lightsail/
- https://aws.amazon.com/es/lambda/features/