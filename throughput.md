# Throughput

**Throughput:** Total number of requests served in a given time interval. E.g., requests per second.

### Causes of Low Throughput:
1. **If latency is high, then throughput is low**, because if the time taken to serve a request is high, then the number of requests served in a given time interval will be less.
2. **Protocol overhead:** If the protocols used to transfer data are not efficient, then the throughput will be low.
   * *Example:* HTTP 1.1 vs HTTP 2.0. HTTP 2.0 is more efficient than HTTP 1.1 because it uses binary framing and multiplexing.
   * **CPU/Memory bottleneck:** If the CPU or memory is not able to handle the requests, then the throughput will be low. Like in protocol overhead, there is a handshake process, and we need to maintain queues or other things; it also causes low throughput.
3. **Congestion control:** If the network is congested, then the throughput will be low. E.g., there is a link that can handle 100 Mbps of data, but we are sending 200 Mbps of data, then the throughput will be low because the link is congested.

### How to Increase the Throughput:
1. **Use efficient protocols:** Use HTTP 2.0 instead of HTTP 1.1.
2. **Increase CPU/Memory:** Increase CPU/Memory of the server.
3. **Reduce latency:** Reduce latency by using a CDN.
4. **Reduce congestion:** Reduce congestion by using congestion control.
5. We can also use CDN and caching to increase the throughput.
6. Use a distributed system in place of a monolithic system.
