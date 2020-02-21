# EC2
Virtual servers in the cloud. Reduces the time required to obtain and boot new server instances to minutes. Allows to quickly scale capacity (up and down) as required

## Pricing models
- On demand
    - Allows you to pay a fixed rate by the hour with no commitmnet
    - Usefull
        -   Users that want the low cost and flexibilitty of amazon ec2 withou any up-front payment or long term commitment
        - Applications with short term, spiky, or unpredictable workloads that cannot be interrupted
        - Application being developed or tested on Amazon EC2 for the first time
- Reserved
    - Provides you with a capacity reservation and offer a significant discount on the hourly charge for an instance. Contract terms are 1 year or 3 years
    - Usefull
        - Applications with steady state of predictable usage
        - Applications that require reserved capacity
        - users able to make upfront payments to reduce their total computing costs even further
    - pricing types
        - Standard
            - There offer up to 75% off on demand instances. the more you pay up front and the longer the contract, the greater the discount
        - Convertible Reserved instances
            - These offer up to 54% off on demand capability to change the attributes of the RI as long as the exchange results in the creation of reserved instances of equal or greater value.
        - Scheduled reserved instances
            - These are available to launch within the time windows you reserve. This option allows you tu match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day, a week or a month
- Spot
    - Enables you to bid whatever price you want for instance capacity, providing fo even greater saving if your applications have flexible start and end times.
    - Useful
        - Applications that hava flexible starts and end times
        - Applications that are only feabile at very low compute prices
        - users with urgent computing needs for large amounts of additional capacity
- Dedicated hosts
    - Physical EC2 server dedicated for your use. Dedicated hosts can help you reduce costs by allowing you to use your existing server-bound software licenses.
    - useful
        - for regulatory requirements that may not support multi-tenant virtualization
        - great for licesing which does not suppoert multi tenancy or cloyud deployments
        - can be purchased on demand
        - Can be purchased as a reservation for up to 70% off the on demand price
## Instances types
|family|speciality|use case|
|:----------:|:---------:|:-----------:|
|F1|field programmable gate array|Genomics research, financial analytics, real time video processing, big data|
|I3|high speed storage|Nosql DBS, data warehousing|
|G3|graphic intensive|Video encoding / 3d application streaming|
|H1|high disk throughput|Map reduce-based workloads, distributed file systems such as hdfs and mapR-FS|
|T3|lower cost, general purpose|Web serves/Small DBs|
|D2|dense storage|Fileservers/data warehousing/hadoop|
|R5|memory optimized|Memory intensive apps/DBs|
|M5|general purpose|Application servers|
|C5|compute optimized|CPU intensive apps/DBs|
|P3|graphics/general purpose gpu|Machine leaning, Bit coin mining|
|X1|memory optimized|SAP HANA/Apache Spark|
|Z1D|high compute capacity and a high memory foorptint|Ideal for electronic design automation (EDA) and certaing relational database workloads|

# EBS
Allows you to create storage volumes and attach them to amazon ec2 instances. Once attached, you can create a file system on top of these volumes, run a database, or use them in any other way you would use a block device. EBS volumes are placed in a specific availability zone, where they are automatically replicated to protect you from the failure of a single component
## Types
- SSD
    - GBeneral purpose SSD (GP2) - Balances price and perfomance for a wide variety of workloads
    - Provisioned IOPSS SSD (IO1) - Highest-perfomance SSD volume for mission-critical low-latency or high-throughput workloads
- Magnetics
    - Throughput optimized hdd (ST1) - Low cost HDD volume designed for frequently accessed, throughput intensive workloads
    - Cold HDD (SC1) - Lowest cost HDD volume designed for less frequently accessed workloads (file servers)
    - Manegtic - Previous generation
### Exam tips
- EC2 is a web service that provides resizable compute capacity in the cloud. reduces the time required to obtain and boot new servers instances to minutes. Allows to quickly scale capacity (up and down) as required
- Pricing models
- If spot instance is terminated by aws EC2, you will not be charge for partial hours of usage. However, if you terminate the instances yourself you wil be charged for any hour in which the instances ran
- F·I·G·H·T·D·R·M·C·P·X·Z
- Volumes type