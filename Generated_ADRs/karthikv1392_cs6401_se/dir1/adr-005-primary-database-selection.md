---
### ADR-005: Primary Database Selection

**Status:** Inferred
**Context:** The application needs to store sensitive user data, financial transactions, account information, savings goals, and user-defined categories. The data is highly relational (e.g., a user has many accounts, an account has many transactions). Data integrity, consistency, and the ability to perform complex queries are paramount.

**Decision:** We will use **PostgreSQL** as our primary database. We will host it on a managed cloud service like Amazon RDS or Google Cloud SQL to handle backups, patching, and scaling.

**Consequences:**
*   **Pros:**
    *   **Reliability & ACID Compliance:** As a mature relational database, PostgreSQL guarantees data integrity through ACID transactions, which is critical for financial data.
    *   **Powerful Querying:** SQL is extremely powerful for generating the complex reports and aggregations required by the dashboard.
    *   **Scalability & Features:** PostgreSQL is highly scalable and supports advanced data types (like JSONB), allowing for flexibility while maintaining a structured schema.
    *   **Managed Service:** Using a managed service like RDS offloads significant operational overhead from the development team.
*   **Cons:**
    *   **Schema Rigidity:** Requires a well-defined schema upfront. While this is generally a benefit for this type of application, it is less flexible for rapidly changing or unstructured data compared to NoSQL alternatives.
    *   **Scaling Complexity:** While vertically and horizontally scalable, scaling a relational database can be more complex than scaling many NoSQL databases at a massive scale. This is not a concern for the initial stages of the project.