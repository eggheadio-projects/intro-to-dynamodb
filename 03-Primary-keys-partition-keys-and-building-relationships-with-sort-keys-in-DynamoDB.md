# [Primary keys vs partition keys and building relationships with sort keys in DynamoDB](https://egghead.io/lessons/aws-primary-keys-vs-partition-keys-and-building-relationships-with-sort-keys-in-dynamodb?pl=intro-to-dynamodb-f35a)

## The composition of a primary key
The primary key for each item in a table must always be unique.

You have the option of creating a table with a primary key that is composed only of a partition key.
- Chris shows that in these tables, no two items can share the same partition key without error.

If you allow the primary key of your table to be composed of both a sort key and a partition key, you can have two or more items with the same partition key, as long as the sort keys differ.

In running a query with a primary key composed of both a partition key and a sort key, it is required that the partition key is specified, but the specification of a sort key is not required.
- "This fairly innocuous feature is what will enable us to build complex single table adjacency lists based designs that replicate the relationship functionality of large SQL tables."

## Resources
["What Is a Primary Key?"](https://www.lifewire.com/primary-key-definition-1019179)
