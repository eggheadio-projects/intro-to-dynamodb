# [WTF are read capacity units (RCU) and write capacity units (WCU) in DynamoDB (Cost $$)](https://egghead.io/lessons/aws-wtf-are-read-capacity-units-rcu-and-write-capacity-units-wcu-in-dynamodb-cost?pl=intro-to-dynamodb-f35a)

## Read and Write Capacity Units
Two Pricing Models:
- Provisioned
  - Definite number of provisioned read capacity units and write capacity units.
- On-Demand
  - Indefinite number of provisioned read capacity units and write capacity units.

One read capacity unit per 4KB of item
- An 8KB item would count as two read capacity units

One write capacity unit per 1KB of item
- A 2KB item would require two write capacity units

Two options for RCUs and WCUs:
- Strongly consistent
- Transactional

Both options double the size of the WCU or RCU
- A strongly consistent or transactional read on a 4KB item would count as two read capacity units.
- Similarly, with transactional writes, a 3KB item would cost six write capacity units.

[Dynobase](https://dynobase.dev/) has a DynamoDB pricing calculator that handles both pricing models.
- The number of WCUs and RCUs, and the amount of data in the table, affects the pricing.

The AWS Free Tier includes 25 WCUs and 25 RCUs of provisioned capacity plus 25GB of data storage.

## Resources
[DynamoDB Pricing Calculator from Dynobase](https://dynobase.dev/dynamodb-pricing-calculator/)

[Read/Write Capacity Mode](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadWriteCapacityMode.html)

[Managing Settings on DynamoDB Provisioned Capacity Tables](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ProvisionedThroughput.html)
