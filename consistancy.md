# Consistency

**Consistency** means data should be consistent. Let's say a person has a bank balance of 100 rupees and he withdraws 10 rupees from one machine. Suppose the other machine doesn't get updated with this transaction, then the balance is not consistent.

Consistency means data should be the same in all distributed systems.

Let's identify where data is consistent: monolithic or distributed systems.

### Factors Improving Consistency:
* Improving network bandwidth so that synchronization becomes faster.
* Stop the read operation until all the servers get updated.
* Replication based on distance-aware strategies.

### Types of Consistency:
1. **Strong Consistency:** When the system does not allow any read operation until the data is updated in all the servers, there is no chance of a dirty read. E.g.: banking transactions.
2. **Eventual Consistency:** When the system allows the read operation even if the data is not updated in all the servers. E.g.: social media, Instagram.
3. **Weak Consistency:** When the system does not guarantee any consistency.