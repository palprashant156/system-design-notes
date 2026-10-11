# Load Balancer

A load balancer is a device or software that distributes network traffic across multiple servers. It acts as a reverse proxy, intercepting client requests and forwarding them to the appropriate server in a server farm or cluster.

### What is Load Balancing?

Load balancing is the process of distributing network traffic across multiple servers to ensure no single server is overwhelmed. It helps improve application availability, scalability, and performance.

### Why Load Balancing?

* Distribute traffic across multiple servers
* Improve application availability
* Improve application scalability
* Improve application performance

# Advantages of Using Load Balancers

1. **Optimisation:** Load balancers help in resource utilisation and lower response time, thereby optimising the system in a high traffic environment.

2. **Better User Experience:** Load balancers help in reducing the latency and increasing availability, making the user's request go smoothly and error-free.

3. **Prevents Downtime:** Load balancers maintain a record of servers that are non-operational and distribute the traffic accordingly, therefore ensuring security and preventing downtime, which also helps increase profits and productivity.

4. **Flexibility:** Load balancers have the flexibility to re-route the traffic in case of any breakdown and work on server maintenance to ensure efficiency. This helps in avoiding traffic bottlenecks.

5. **Scalability:** When the traffic of a web application increases suddenly, load balancers can use physical or virtual servers to deliver the responses without any disruption.

6. **Redundancy:** Load balancing also provides in-built redundancy by re-routing the traffic in case of any failure.



# Load Balancing Algorithms

1. **Round Robin (Static):** Requests are distributed among servers in a rotational fashion.

2. **Weighted Round Robin (Static):** It is similar to the Round Robin algorithm, but it is used when servers have different capacities. Some nodes may have better resources than others.

3. **IP Hash Algorithm (Static):** The servers have almost equal capacity, and a hash function (with the source IP as input) is used for the random or unbiased distribution of requests to the nodes.

4. **Source IP Hash (Static):** Source IP Hash combines the server and client's source and destination IP addresses to produce a hash key. The key can be used to determine the request distribution.

5. **Least Connection Algorithm (Dynamic):** Client requests are distributed to the application server with the least number of active connections at the time the client request is received.

6. **Least Response Time (Dynamic):** The request is distributed based on the server that has the least response time.