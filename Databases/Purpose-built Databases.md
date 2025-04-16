These DBs are catered towards specific use cases

- [[DynamoDB]] : Fully managed NoSQL, flexible, consistent and catered to high scale or/and serveless applications. (It can also work for nearly all online transaction processing - OLTP)]
- [[Amazon Elasticache]] : Fully managed, in-cache solution, supports Redis and MemCached
- Amazon MemoryDB for Redis: Fully compatible with Redis, offer milisecond latency and multi-az durability. Can be used as a primary db for high perfomance apps
- [[DocumentDB]]: Fully managed, NoSQL useful for content management systems, profile management and web/mobile apps. MInimal hassle for migrating into.
- Amazon Keyspaces: Compatible with Apache Cassandra, good option for high volume apps with straightfoward access patterns
- [[Amazon Neptune]]: Fully managed graph database offered by AWS. Good choice for highly connected data with a variety of relationships. Recomended for recomendation engines, fraud detection and knowledge graphs
- [[Amazon Timestream]]: Serverless DB for Internet of Thing (IoT). Can store and analyze trillions of events per day faster than and cheaper than relational databases. Useful for tracking events that changes overtime such as stock prices, temperatures and other measurements
- [[Amazon QLDB]]: Ledger Database that provides complete and cryptographically verifiable history of changes made to the app data.