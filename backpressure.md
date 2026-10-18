# Backpressure

Back pressure means: when a system is overloaded, it tells the system sending it work to slow down.

2. How it works in a distributed system
Imagine your application has three services:
Service A — Producer
Sends 1,000 requests/second

Queue / Message Broker
Requests start piling up

Service B — Consumer
Can process only 200 requests/second


Back pressure signal
"I'm overloaded. Send fewer requests."



Without back pressure, requests keep accumulating, memory usage increases, response times become slower, and eventually the service may crash.
With back pressure, Service B signals that it cannot handle more work, and Service A slows down or sends fewer requests.
3. What happens without vs. with back pressure?
Without back pressure	With back pressure
Requests keep piling up	Incoming work is controlled
Memory usage may grow	Memory stays more manageable
Response times increase	System can remain responsive
Service may crash	Service has a better chance to recover
4. How do developers implement it?
Common techniques include:
- Rate limiting: Allow only a certain number of requests per second.
- Bounded queues: Limit how many requests can wait in a queue.
- Throttling: Slow down the rate at which work is sent.
- Load shedding: Reject or discard lower-priority work when overloaded.
- Reactive streams: Signal upstream components to produce data more slowly.