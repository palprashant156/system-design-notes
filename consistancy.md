consistancy: means data should be consistant let say a person have bank balance of 100 rupee and he withdraw 10 rupee from one machine suppose the other machine doesn't get updated with this transaction then the balance is not consistant.

consistancy means data should be same in all the distributed system.

lets identify where data is consistant monolithic or distributed system.

Factor improving consistancy:
improving network bandwidth so that synchromization become faster.
Stop the read operation until all the server get updated.
Replication based on distance aware strategies.
Types of consistancy:
1. Strong consistancy:when system doesnot allow any read operation until the data is not updated in all the server,there is no chance of dirty read.eg:banking transaction.
2. Eventual consistancy:when system allow the read operation even if the data is not updated in all the server.eg:social media,instagram.
3. Weak consistancy:when system doesnot guarantee any consistancy.