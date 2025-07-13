# 🏗️ System Design Interview Questions & Answers

### Q1: What is system design?
- A: It’s the process of defining the architecture, components, modules, interfaces, and data for a software system.

### Q2: Difference between monolith and microservices?
- A: Monolith is a single codebase; microservices split functionality into independent services.

### Q3: When to use microservices?
- A: When scaling independently, having clear service boundaries, or needing language/database flexibility.

### Q4: What is load balancing?
- A: Distributing incoming traffic across multiple servers to ensure no single server is overwhelmed.

### Q5: Horizontal vs vertical scaling?
- A:
    - Horizontal: Add more servers
    - Vertical: Upgrade a server's CPU/RAM

### Q6: What is CDN?
- A: Content Delivery Network – delivers static assets from edge locations closer to users.

### Q7: What is a cache?
- A: Temporary data store (e.g. Redis, Memcached) to reduce DB calls and improve performance.

### Q8: Cache eviction policies?
- A: LRU, LFU, FIFO.

### Q9: What is database sharding?
- A: Splitting a database into smaller pieces distributed across servers.

### Q10: What is replication?
- A: Copying data from master to one or more replicas for redundancy and performance.

### Q11: What is a message queue?
- A: Asynchronous communication between services using systems like RabbitMQ, Kafka, or SQS.

### Q12: When to use queues?
- A: For background processing, retrying failed jobs, rate limiting.

### Q13: What is eventual consistency?
- A: System guarantees data consistency eventually, not instantly.

### Q14: What is CAP theorem?
- A: You can only choose two of: Consistency, Availability, Partition Tolerance.

### Q15: What is a reverse proxy?
- A: A server (e.g., NGINX) that routes requests to backend services, often with caching or SSL termination.

### Q16: What is a service discovery system?
- A: Automatically tracks available services in dynamic environments (e.g. Consul, Eureka).

### Q17: What is the role of API gateway?
- A: Handles routing, authentication, rate-limiting, and aggregation for microservices.

### Q18: Difference between REST and GraphQL?
- A:
    - REST: Multiple endpoints, fixed structure
    - GraphQL: One endpoint, client defines structure

### Q19: How do you secure a distributed system?
- A: Use TLS, API keys, OAuth, service-to-service authentication.

### Q20: What is idempotency?
- A: Performing the same operation multiple times results in the same outcome.

### Q21: What are rate limiters?
- A: They restrict how many requests a user/client can make within a time frame.

### Q22: What is circuit breaker pattern?
- A: Stops calling a failing service temporarily to allow it to recover.

### Q23: What is a fallback mechanism?
- A: An alternative flow when a service or resource is unavailable.

### Q24: How do you prevent cascading failures?
- A: Use circuit breakers, timeouts, bulkheads, and retries with backoff.

### Q25: What is database partitioning?
- A: Dividing a database into parts to optimize performance (by range, list, hash).

### Q26: What is schema-less design?
- A: Common in NoSQL (e.g., MongoDB), allows flexible and dynamic structures.

### Q27: When to choose SQL vs NoSQL?
- A:
    - SQL: Strong consistency, structured data
    - NoSQL: Scalability, unstructured or rapidly changing data

### Q28: What is a design for a chat application?
- A: Requires WebSockets, presence tracking, message queues, and Redis for pub/sub.

### Q29: What is a design for a payment system?
- A: Wallet service, transaction logs, audit trail, fraud detection, retry queues.

### Q30: What is eventual vs strong consistency?
- A:
    - Strong: All clients see latest data instantly
    - Eventual: Data converges over time

### Q31: What is a rate limiter algorithm?
- A: Token bucket, Leaky bucket, Fixed window, Sliding window.

### Q32: How to store large files?
- A: Use object storage (e.g., AWS S3) and serve via signed URLs or CDNs.

### Q33: What is object storage vs block storage?
- A:
    - Object: For unstructured data (S3, MinIO)
    - Block: For disks (used in VMs)

### Q34: How to design an upload service?
- A: Use chunked uploads, background virus scanning, and CDN integration.

### Q35: What is the role of Redis in system design?
- A: Caching, pub/sub, queueing, distributed locks.

### Q36: What is eventual delivery guarantee?
- A: Ensures messages will be delivered at least once.

### Q37: Difference between at-least-once vs at-most-once delivery?
- A:
    - At-least-once: May repeat
    - At-most-once: May miss

### Q38: What is consistency hashing?
- A: Distributes data evenly when nodes are added/removed.

### Q39: What are distributed transactions?
- A: Coordinating transactions across multiple services or databases.

### Q40: What is SAGA pattern?
- A: Manage long-lived transactions with compensating steps across services.

### Q41: What is database indexing?
- A: Speeding up data lookups using structures like B-Trees.

### Q42: How would you design an API rate limiter?
- A: Use Redis with IP/user as key, increment counter per request, expire in time window.

### Q43: What is high availability?
- A: Minimizing downtime via redundancy, failover, replication.

### Q44: What is autoscaling?
- A: Automatically adjusting the number of instances based on traffic.

### Q45: What is infrastructure as code (IaC)?
- A: Managing infra with code (e.g., Terraform, Pulumi, CloudFormation).

### Q46: What are blue-green deployments?
- A: Reduce downtime by deploying new version on parallel infra, then switching traffic.

### Q47: What is CI/CD?
- A: Continuous Integration & Delivery/Deployment for automating build/test/deploy.

### Q48: What is Docker used for?
- A: Containerizing apps for portability, consistency, and isolation.

### Q49: What is Kubernetes?
- A: Container orchestration system for managing deployments, scaling, and networking.

### Q50: How do you monitor a distributed system?
- A: Use tools like Prometheus, Grafana, ELK stack, APMs (Datadog, New Relic).

