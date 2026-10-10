# System Design: Scalability

### Vertical Scaling
Vertical scaling means we are just increasing the resources of the CPU (adding more resources to your existing server like RAM, CPU, storage).

We cannot add physical resources to our running machine, so we have to restart the server. In that case, downtime occurs. And one more thing, here a single IP is there, that’s why we don’t need a load balancer.

* **Cons:** Ideally, downtime should be zero.

### Horizontal Scaling
Horizontal scaling means we are just increasing the resources just by adding a copy of the existing server. So in this case, we need to add a load balancer in between two servers (copies/replicas) because here multiple IPs are there due to the load balancer.

### Serverless Architecture
In serverless architecture (Lambda), when any API is hit and sudden traffic comes, it just makes a replica of Lambda. But the first time when any request comes, Lambda will warm up for a few seconds. For limited, predictable daily active users, like if you have 100 subscribers, in this case, Lambda will never go deep cold.

* **Note:** Where we manage it, it's called serverful architecture, and where the cloud manages it, it's serverless architecture.

#### AWS Lambda
In serverless (AWS Lambda), when an API gets hit, Lambda runs your function.
* If sudden traffic comes, AWS automatically creates more Lambda copies (instances).
* The first time after being idle, Lambda takes a few seconds to start → this is a **cold start**.
* After that, Lambda stays active for some time → next requests are fast (**warm start**).
* If requests keep coming regularly, Lambda usually doesn’t go deep cold.
* But AWS doesn’t guarantee always warm — a cold start can still happen sometimes.

**Pros:** 1 million free, very cheap.
**Cons:** Cold start.

* Required API: that’s why the duration is fixed, you cannot take more than 15 seconds to return a request.
* Due to DDoS attacks, scaling can run infinite times.
* Vendor lock-in: once you structure your code according to Lambda, you cannot move to other clouds like DigitalOcean.
* It starts using SQS (Simple Queue Service), a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.

### Event Sourcing
* **Event:** When something is uploaded or downloaded, or some kind of clicks happen, it's called an event.