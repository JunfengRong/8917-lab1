
## Investigate Azure Database Services

Here is a concise English explanation for each item.

1. Azure Cosmos DB
- What is it?

    A globally distributed, fully managed NoSQL database designed for low latency and massive scalability.

- What data models does it support?
    
    - Document (Core SQL API)
    - Key–value (Table API)
    - Column‑family (Cassandra API)
    - Graph (Gremlin API)
    - MongoDB API (document)
    
- What is the serverless tier?

    A consumption‑based mode where you pay only for actual request units (RUs) used, with no pre‑provisioned throughput.

2. Azure Table Storage
- What is it?

    A simple, low‑cost key–value NoSQL store for large amounts of semi‑structured data.

- How does it differ from Cosmos DB?
    - Table Storage is cheaper, but has fewer features
    - Cosmos DB Table API is faster, globally distributed, and supports automatic indexing
    - Table Storage has no SLA for latency, no global distribution, and limited querying
- When is it appropriate?
    - When you need very cheap, simple key–value storage
    - When global distribution, advanced queries, or low latency are not required

3. Azure SQL Database
- What is it?
    - A fully managed relational database based on Microsoft SQL Server, supporting SQL queries, transactions, and strong consistency.
- When choose SQL over NoSQL?
    - When your data has relationships
    - When you need ACID transactions
    - When you require complex joins, stored procedures, or strong schema
    - When analytics or reporting depend on structured data

4. Azure Blob Storage
- Can it be used as a database?

    - Not a database, but it can store data files (JSON, CSV, images, logs).
    - Some applications treat it as a “data lake,” but it lacks database features.

- What are the trade‑offs?

    | Pros | Cons|
    |------|-----|
    |Extremely cheap | No querying|
    | Massive scale | No indexing| 
    |Great for unstructured data | No transactions|
    |Ideal for backups, logs, media | Not suitable for relational or NoSQL workloads|

## Database Choice: 
1. Which database did you select?
   I selected Azure Cosmos DB.
2. Justification: Why is this the best choice for this use case? (3-5 sentences)
    - Cosmos DB is globally distributed, with low latency and high availability.
    - It supports multiple APIs, including Document, Key-Value, Column-Family, Graph, and MongoDB.
    - It has a serverless tier, which means you only pay for actual usage.
3. Alternatives Considered: What other options did you evaluate and why did you reject them?
    - Azure Table Storage: Cheaper, but lacks features like global distribution and advanced querying.
    - Azure SQL Database: Expensive, but suitable for relational workloads with complex queries.    
4. Cost Considerations: How does pricing work for your chosen database?
    - Cosmos DB: Pay-as-you-go model, with no upfront costs. You pay only for actual request units (RUs) used.
    - Table Storage: Cheaper, but you pay for storage and requests.
    - SQL Database: Expensive, with a pay-per-hour model. You pay for compute resources and storage.


