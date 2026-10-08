CAP:

* **C - Consistency**: Data should be consistent in all the distributed systems.
* **A - Availability**: Availability means the system should be available to serve the requests.
* **P - Partition Tolerance**: Partition tolerance means the system should be able to handle the network partitions.

In distributed systems, we can only have two of the three properties. 
We cannot have all the three properties at the same time.

* Let's say if we choose consistency and availability, partition tolerance would be compromised.
* If availability and partition tolerance are chosen, then consistency will be compromised. 
* If we choose partition tolerance and consistency, then availability would be compromised.

So, at a time, only two can be achieved at a time: either CA, AP, or CP. But why? Let's understand.

**CP (Consistency and Partition Tolerance)**
If we choose CP, then availability would be compromised because in a distributed system, a lot of nodes will be there. So, if anyone makes changes in one node, then it will take time to update the things in other nodes as well, and maybe someone is also changing the things in other nodes, so we have to stop (compromise) the availability. E.g., banking transactions.

**AP (Availability and Partition Tolerance)**
If we choose AP, then consistency would be compromised because in a distributed system, a lot of nodes will be there. Let's understand with an example: if any social media is there, if anyone (node) posts something, it is okay to receive the notification with a little bit of delay because it is not a very important thing. So, here consistency can be compromised.

**CA (Consistency and Availability)**
If we choose CA, then partition tolerance would be compromised because in a monolithic system, single nodes will be there. Let's understand with an example: if one database is there, in that database data is continuously coming, so it is available, and due to live data, consistency is automatically there. But if the database goes down, then we cannot achieve partition tolerance.