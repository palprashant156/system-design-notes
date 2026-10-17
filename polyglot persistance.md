# What is a Polyglot Database?

Polyglot persistence is a system design approach in which an application uses multiple types of databases to store different kinds of data, choosing each database based on the specific requirements of that data.

In simple words, instead of using one database for everything, you use different databases for different purposes.

---

### 1. Real-World Example
Imagine you are building an e-commerce application like Amazon.

**E-commerce Application:** Users · Products · Orders · Payments

* **PostgreSQL:** Users, orders, payments, and transactions
* **MongoDB:** Flexible product catalogs and attributes
* **Redis:** Cache, sessions, and temporary data
* **Elasticsearch:** Full-text product search and filtering

Each database serves a different purpose within the same application.

---

### 2. Why Use Multiple Databases?

| Requirement | Suitable Database | Why? |
| :--- | :--- | :--- |
| Financial transactions | PostgreSQL | ACID transactions and relational constraints |
| Flexible document data | MongoDB | Document-oriented storage |
| Fast caching | Redis | In-memory data access |
| Full-text search | Elasticsearch | Text indexing and relevance-based search |
| Relationship-heavy graph queries | Neo4j | Efficient graph traversal |

These are common choices, not strict rules. Some databases can support several of these workloads.

---

### 3. How Does It Work in a Backend Application?
Suppose you are using NestJS.

**NestJS API:** Controllers and services

* **OrderService** → TypeORM → PostgreSQL
* **CacheService** → Redis client → Redis