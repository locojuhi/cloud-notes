# Cloud front 
A content delivery network (CDN) is a system of distributed servers (network) that deliver webpages and other web content to a user bsed on the geographic locations of the user.
Can be used to deliver your entire website, including dynamic, static, streaming and interactive content using global network of edge locations. Requests for your content are automatically routed to the nearest edge location.

### Edge location
This is the location where the content will be cached. This is separate to an AWS region/AZ.

### Origin
This is the origin of all the files that the CDN will distribute. This can be an S3 bucket, an EC2 instance and Elastic load balancer or Route53

### Distribution
This is the name given then CDN which consists of a collection of edge locations.

### Terminology
- Web distribution - Typically used for websites
- RTMP - Used for media streaming

### Exam tips
- Edge location
- Origin
- Distribution
    - Web distribution
    - RTMP
Edge location are not just RAED only - You can write to them too
- Objects are cache for the life of the TTL
- You can clear cached objects, but you will be charged