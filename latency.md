# Latency

**Latency:** The time taken for data traveling end-to-end. E.g., from one client to a server.

### Typical Latency Values
Typically, latency will be in ms (milliseconds). And network latency can be calculated using the formula:

**Latency = Distance / Speed**

Latency means: `Network Delay + Computation Delay + Processing Delay + Queueing Delay`.

### Reducing Latency
For reducing the latency, we can use caching and CDN. Here caching means storing the requested response of the client in cache memory, so that next time if the same client requests the same response, it can be served from the cache memory itself, and it will be faster than the original response from the server.

### Typical Latency Values (Round Trip Time):
* **LAN:** 1 ms
* **WAN:** 100 ms

And a CDN can reduce the latency by serving the response from the nearest server. E.g., if the client is in India and the server is in the USA, then the CDN will serve the response from the nearest server to the client. 
And CDN means Content Delivery Network. E.g., when we open youtube.com in India, it will serve the response from the nearest server to the client, which can be in India or nearby. This reduces the latency.
