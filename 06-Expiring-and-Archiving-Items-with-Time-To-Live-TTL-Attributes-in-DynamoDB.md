# [Expiring and Archiving Items with Time To Live (TTL) Attributes in DynamoDB](https://egghead.io/lessons/aws-expiring-and-archiving-items-with-time-to-live-ttl-attributes-in-dynamodb?pl=intro-to-dynamodb-f35a)

## The Time to Live Attribute
Enabling Time to Live on a DynamoDB table allows you to specify when an item will be deleted from the table.
- The value of this attribute must be a Unix timestamp in seconds

It is not guaranteed that an item will be deleted immediately with TTL
- If timing is critical for your application, use a filter expression on any of your queries to filter out items with an expired TTL value

The name of the TTL attribute doesn't matter, but the value must be a number.
- The name of the TTL attribute is then specified when enabling TTL.

Items with no TTL attribute will stick around forever.

If the "Enable with view type New and old Images" box is checked when enabling TTL, "when items get deleted, they will get pushed to a DynamoDB stream which gives us 24 hours to process them and archive them perhaps to S3 if we want to.

Hovering over the TTL value will give you the UTC, Local Time, and Region Timestamp equivalent.

## Resources
[EpochConverter Timestamp Conversion Tools](https://www.epochconverter.com/)
