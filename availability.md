# Availability

Let's say today CBSE announces the results and a lot of students check the results; suddenly the website goes down.

Let's figure out which one has high availability: monolithic vs. distributed.

* **In Monolithic:** All the things are deployed on 1 server. And suppose, if the server is down, then the website will go down. This means the whole thing will go down, and the whole service stops.
* **In Distributed:** Every service is deployed on a different server. Suppose if one server is down, then the other server will work properly. So the website will not go down. This means 1 service is down, but the other service will work properly.

As a result, after figuring it out, the availability is high in a distributed system.

Fault tolerance is directly proportional to availability.

### How to Increase the Availability?
* **Answer:** Replication is nothing but making a copy of data on a different server.
* A distributed system is used for high availability.
* **Redundancy:** Redundancy is nothing but having multiple copies of the same thing. Such as multiple servers, multiple databases, multiple power supplies, etc.
* By adding more machines, we can increase the availability.
* Redundancy is the duplication of nodes; in case some of them are failing, we can use the other nodes.