CAP:
C: consistancy: data should be consistant in all the distributed system.
A: Availability: availability means the system should be available to serve the requests.
P: Partition Tolerance: partition tolerance means the system should be able to handle the network partitions.

In distributed system, we can only have two of the three properties. 
We cannot have all the three properties at the same time.

let say if we choose consistancey and availability partition tolerance would be compromised
if availability and partion tolerance will be choose then consistancey will be compromised 
if we choose partition tolerance and consistancey then availability would be compromised

so at a time only two can achive at a time either CA OR AP OR CP but why lets understand

if we choose CP then Availability would be compromised because in distributed system lot of nodes will be there so if anyone make changes in one node then it will take time to update the things in other nodes as well and may be someone is also changing the things in other nodes so we have to stop(compromised) the availability. eg:banking transaction.



if we choose AP then consistancy would be compromised because in distributed system lot of nodes will be there lets understand with the example if any social media is there if anyone(node) post something it is ok to recevice the notification little bit delay becuase it is not a very important thing so here consistancey can be compromised



if we chose CA then partition tolerace would be compromised because in monolithic system single nodes will be there lets understand with the example if one database is there in that database data is continuously coming so it is available and due to live data consistance is automatically there but if database is go down then we cannot achieve the partition tolerace.