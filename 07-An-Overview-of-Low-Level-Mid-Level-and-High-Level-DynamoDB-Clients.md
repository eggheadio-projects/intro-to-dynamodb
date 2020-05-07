# [An Overview of Low-level, Mid-level (Document), and High-level DynamoDB Clients](https://egghead.io/lessons/aws-an-overview-of-low-level-mid-level-document-and-high-level-dynamodb-clients?pl=intro-to-dynamodb-f35a)

## Abstraction in DynamoDB
The level of abstraction of the DynamoDB interface depends on the language you're using, and ranges from low-level, to document, to high-level.

The Object Persistence Interface is the highest level interface and is only available for Java and .NET
- Allows you to interact with Java objects and classes instead of the database

The Document Interfaces are more widely supported, and allow you to take advantage of the abstraction of objects in your language of choice.
- Requires explicit methods to interact with DynamoDB itself

Low-Level Interfaces require more work and specification.
- Doesn't automatically translate from your programming language of choice to DynamoDB types.

## Resources
[A Detailed Explanation of Abstraction in Software Development](https://thevaluable.dev/abstraction-software-development/)
