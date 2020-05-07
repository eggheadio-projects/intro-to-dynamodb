# [An Introduction to DynamoDB Global Secondary Indexes (GSIs)](https://egghead.io/lessons/aws-an-introduction-to-dynamodb-global-secondary-indexes-gsis?pl=intro-to-dynamodb-f35a)

## Global Secondary Indexes
Chris begins this lesson with an example of a table in which the primary key is composed of a partition key and a sort key.

Chris shows that, in running a query, one can specify only the partition key, or both the partition key and the sort key, but cannot specify only the sort key.

"GSIs allow us to query efficiently over any field (attribute) in our DynamoDB table. GSIs can treat any table attribute as a key, even attributes not present in all items."

Chris, in creating an index, specifies the partition key as "sk", and chooses to project all attributes.
- You also have the ability to project only the keys or specify exactly what attributes should be returned.
- You must also specify the read capacity units and the write capacity units. This will come at a price.

Now, through the use of indexes, we can return items through the specification of only the sort key.

"A secondary index is basically a copy of our data stored in a different way, that allows us to access it in a different way."

The maximum number of GSIs per table is 20, but you'll likely never need more than 5.

Items that don't have an attribute specified by the index will not be indexed.

Creating GSIs
- Allows us to specify a partition key and a sort key that can be made out of any of our attributes
- Lets us take specific attributes and move them into that index depending on what we actually want back from that index query.

## Resources
[Using Global Secondary Indexes in DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GSI.html)

[What is a Database Query?](https://www.lifewire.com/query-definition-1019180)
