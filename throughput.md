throughput: total number of requests served in a given time interval. e.g. requests per second.
causes of low throughput
1. if latency is high then throughput is low, because if the time taken to serve a request is high then the number of requests served in a given time interval will be less.
2. protocol overhead: if the protocols used to transfer data are not efficient, then the throughput will be low.
Example: http 1.1 vs http 2.0. http 2.0 is more efficient than http 1.1 because it uses binary framing and multiplexing.
cpu/memory bottleneck: if the cpu or memory is not able to handle the requests, then the throughput will be low.
like in protocol overhead there is handshake process , we need to maintain queue or other things it is also cause low throughput.
3. congestion control: if the network is congested, then the throughput will be low. e.g. there is a link that can handle 100mbps of data, but we are sending 200mbps of data, then the throughput will be low because the link is congested.

how to increase the throughput:
1. use efficient protocols: use http 2.0 instead of http 1.1
2. increase cpu/memory: increase cpu/memory of the server
3. reduce latency: reduce latency by using cdn
4. reduce congestion: reduce congestion by using congestion control
5. we can also use cdn and caching to increase the throughput.
6. use distributed system in place of monolithic system.
