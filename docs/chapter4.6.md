# Athena

Interactive query service which enables you to analyse and query data located in S3 using standard SQL
- Serverless, nothing to provision
- pay per query / per TB scanned
- No need to set up complex extract/transform/load processes
- works directly with data stored in S3

## Used for
- query log files stored in s3
- Generate business reports on data stored in S3
- Analyse AWS cost and usage reports
- Run queries on click-stream data

# Macie
## PII Personally Identifiable Information (PII)
- Personal data used to establish an individuals identity
- This data could be exploted by criminals, used to indentity therft and financial fraud
    - Home address
    - Email address
    - Passport number
    - phone number
    - credit card number

## Macie
Security service which uses machine learning and NLP (Natural Language Processing) to discover, classify and protect sensitive data stored in S3
- use AI to recognise if your s3 objects contain sensitive data such as PII
- Dashboards, reporting and alerts
- Works directly with data stored in S3
- Can also analyze cloud trail logs
- Great for PCI-DSS and preventing ID theft