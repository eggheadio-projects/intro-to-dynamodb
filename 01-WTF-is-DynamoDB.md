# [01. WTF is DynamoDB?](https://egghead.io/lessons/aws-wtf-is-dynamodb?pl=intro-to-dynamodb-f35a)

## DynamoDB Features
DynamoDB is a key-value and document NoSQL database.

You can expect:
- Low-latency
- Serverless-compatible
- Handles immense scale
- Comes with standard database features
  - Encryption at rest
  - On-demand backup and restore
  - A transparent caching layer
- Faster than millisecond performance
- Fully managed
- Variety of pricing models
- Standard SLA specifies 99.99% uptime, or about 1 hour of downtime in a year.
- Automated backup and restore with Point-in-Time Recovery
- Expiring items using Time to Leave (TTL) Attributes
- Global Tables: Can replicate your DynamoDB table in many AWS regions
- Transactions: Can guarantee higher consistency modeling for reads and writes
- DynamoDB Accelerator: An in-memory cache that can get you from millisecond response times to microsecond response times
Unlike SQL databases, DynamoDB typically requires you to know your access patterns beforehand.

DynamoDB is not a good choice if you don't know your access patterns, or you need an analytical database.

Service Level Agreement specifies 99.999% uptime (about 5 minutes of downtime) in a year for features like global tables.

DynamoDB is showing up in a lot of Amazon's new architectures, and even supports their core business.

There are GUI clients as well as the CLI and programming language clients for accessing DynamoDB
- NoSQL Workbench allows you to data model DynamoDB schemas
- Dynobase allows you to access all your production DynamoDB instances in various regions

DynamoDB is great for serverless applications when you know that you might need low latency, and you know the access patterns that you're going to use.

## Resources
[Dynobase](https://dynobase.dev/)

[NoSQL Workbench for Amazon DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/workbench.html)

[Data Access Patterns](https://medium.com/mastering-software-engineering/data-access-patterns-the-features-of-the-main-data-access-patterns-applied-in-software-industry-6eff86906b4e)

[What Is a Key-Value Database?](https://aws.amazon.com/nosql/key-value/)

[What is NoSQL?](https://aws.amazon.com/nosql/)

[Awesome DynamoDB](https://github.com/alexdebrie/awesome-dynamodb)

[AWS re:Invent 2019 - Amazon DynamoDB deep dive: Advanced Design Patterns](https://www.youtube.com/watch?v=6yqfmXiZTlM)
