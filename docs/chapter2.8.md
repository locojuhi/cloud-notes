# S3 101

## What is S3
provides developert and IT teams with secure, durable, highly-scalable object storage. easy to use, simple web interface to store and retrieve any amount of data from anywhere on the web.
On resume, It's a place to store any file that you want.

- S3 is a safe place to store your files
- It is Object-base storage
- The data is spread accoss multiple devices and facilities
- files can be from 0 bytes to 5 TB
- There is unlimited sotrage
- Files are stored in buckets (bucket is a folder in the cloud)
- S3 is a universal namespace, so the name must be unique globally
- When upload a file to s3 will receive a http 200 status code

### objects
 - key (name of the object)
 - value (the data made up of a secuence of bytes)
 - version Id (important for versioning)
 - Metada (data that you are storing)
 - Subresources
    - Access Control Lists
    - Torrent

### Data consistency
- Read after Write consistency for puts of new objects
    - If you write a new file and read it immediately afterwards, you will be able to view that data.
- Eventual consistency for overwirte puts and Deletes (can take some time to propagate)
    - If you update an existing file or delete a file and read it immediately, you may get the older version, or you may not. Basically changes to objects can take alittle bit of time to propagate.

### Guarantees
- built for 99.99% availability for s3 platform
- Amazon guarantee 99.9% availavility
- Amazon guarantee 99.999999999% durability for s3 information (remember 11 x 9s)

### Features
    - Tiered Storage Available
    - Lifecycle management
    - Versioning
    - Encryption
    - Secure your data using Access control list and bucket policies

### Storage classes
- s3 standard
    - 99.99% availability
    - 99.999999999% durability stored redundant across multiple devices
- s3 - IA (infrequently accessed)
    - For data that is accessed less frequently, but requires rapid access when needed. lower feed that s3, but you charged a retrieval free.
- s3 One zone - IA
    - lower-cost option for infrequetly accessed data, but do not required the multiple AZ resilence
- s3 - Intelligent Tiering
    - Optimi9ze costs by automatically moving data to the most cost-effective access tier
- s3 Glacier
    - low cost storage for data archiving. retrieval times configurable from minutes to hours
- s3 Glacier Deep Archive
    - lowest cost storage. retrieval time 12 hours is acceptable.

    Notes: 
    - Availability zones >= 3
### charges
- Storage
- Requests
- Storage management pricing
- Data transfer pricing
- Transfer acceleration
- Cross region replication pricing
#### Transfer acceleration
Enables fast, easy and secure transfer of files over long distances between your end users and an S3 bucket. Uses amazon cloudfront

### Exam tips
- S3 is object based
- files can be from 0 bytes to 5 tb
- unlimited storage
- files are storages in buckets
- s3 is a universal namespace
- not suitable install OS
- success upload return 200
- fundamentals are
    - Key (name of file)
    - value (data made up from bytes)
- Read after Write consistency for puts of new objects
    - If you write a new file and read it immediately afterwards, you will be able to view that data.
- Eventual consistency for overwirte puts and Deletes (can take some time to propagate)
    - If you update an existing file or delete a file and read it immediately, you may get the older version, or you may not. Basically changes to objects can take alittle bit of time to propagate.
- Storage classes (see above)

### Aditional exam tips
- Bucket names sahre a common ranme space. you cant have the same bucket name
- when you view you buckets you view them globally but you can have bucket in individual regions
- You can replicate the contents of one bucket to another region bucket by using cross region replication
- You can change storage classes and encryption of objects on the fly
- Restricting bucket access
    - Bucket policies (applies across the whole bucket)
    - Object policies (applies to individual files)
    - IAM Policies to Users and Groups (aplies to users and groups)