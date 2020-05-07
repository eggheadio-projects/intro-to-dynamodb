# [Overview of DynamoDB Tables, Items, Attributes, and types in the AWS console](https://egghead.io/lessons/aws-overview-of-dynamodb-tables-items-attributes-and-types-in-the-aws-console?pl=intro-to-dynamodb-f35a)

## Tables, Items, Attributes, and types in the AWS console
Three core components of a DynamoDB table:
- Tables
- Items in those tables
- Attributes

The entire list of items is the table, and these items map fairly seamlessly to tables in other databases.

Through the text option, the item can be shown as a JSON file

Tables hold items, or JSON objects, and items contain attributes
- Top level keys in items are attributes.
- Sub-keys are not called attributes.

By checking the "DynamoDB JSON" button, you can see all the type information of the item.
- The type information is displayed as one letter i.e. "S" for string, "M" for map (or JSON object), and "N" for number.

"We can think of [tables] as buckets of JSON objects that we can access by key and have attributes that we can query on and values that we can return."

## Resources
[Core Components of Amazon DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.CoreComponents.html)

[Anatomy of an Item](https://www.dynamodbguide.com/anatomy-of-an-item/)
