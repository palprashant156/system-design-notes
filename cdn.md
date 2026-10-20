# CDN (Content Delivery Network)

## Definition

A **Content Delivery Network (CDN)** is a geographically distributed network of servers that delivers web content to users from a server (often called an edge server or point of presence) close to them. CDNs cache copies of content such as images, videos, stylesheets, JavaScript, and downloadable files. When content is not available in the cache, the CDN fetches it from the origin server and may cache it for later requests.

## Uses

- **Reduce latency:** Serve content from a nearby edge location instead of making every user request travel to the origin server.
- **Reduce origin load and bandwidth costs:** Reuse cached content for many users, reducing repeated requests to the application or storage servers.
- **Deliver large files and media efficiently:** Distribute images, software downloads, and video or audio streams across locations.
- **Improve availability and resilience:** Handle traffic spikes and, depending on the CDN configuration, continue serving cached content during some origin outages.
- **Add security protections:** Many CDNs offer DDoS mitigation, web application firewall rules, and TLS termination.

CDNs are especially useful for globally accessed websites and applications. Frequently changing or private content needs suitable cache rules so users do not receive stale or unauthorized data.
