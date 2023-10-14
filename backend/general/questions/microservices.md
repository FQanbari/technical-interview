# Microservices

* What are monolith's downsides and advantages?
* What are microservices downsides and advantages?
* Service Registry & Discovery
    * What's service registry?
    * Tools for service-discovery (Consul, Redis, ...)
    * Where do we need them?
* Load-Balancing
    * What are the application requirements for load-balancing?
    * What's HA?
    * What's replication?
    * What's sharding?
    * What is the difference between Horizontal-Scaling and Vertical-Scaling?
* Distributed Transactions
    * What's SAGA?
    * What's two-phase commit?
* Metrics, Monitoring, Tracing, Logging
    * What's CorrelationId?
    * What's distributed tracing? Why we need that?
    * What are metrics? How to collect them?
    * What's monitoring? How it's related to the metrics?
    * What's centralized logging?
        * What's ELK?
        * How to keep the logs while the logging provider is down?
* Key-Vaults
    * Where to store secret things like passwords, api-keys, ...?
    * What's key-vault?
* Service-Mesh
    * What's service-mesh? Why we need that?
    * What's Side-Car pattern?
* Communication Patterns (Inbox/Outbox, Fan-in/Fan-Out, Pub/Sub, Peer-2-Peer, ...)
    * How microservices can talk to each other?
    * What's gRPC? What's protobuf?
* Message Delivery Semantics (At-Least-Once, At-Most-Once, Exactly-Once) + Retry
    * What's at-least-once in messaging?
    * What's at-most-once in messaging?
    * How to achieve exactly-once delivery in messaging?
    * What should we do when a message not get delivered?
    * What's retry pattern?
 

# Answer

Certainly, let's delve into these topics in more detail.

### Monolith Architecture

### Advantages:

1. **Simpler Development Workflow**: Easier to develop, test, and deploy as everything is in a single codebase.
2. **Transaction Management**: Easier to manage transactions as you're dealing with a single, unified database.
3. **Data Consistency**: Easier to maintain strong consistency due to the single database and synchronous calls.

### Downsides:

1. **Limited Scalability**: Hard to scale individual components separately. You often have to scale the entire application.
2. **Long Build and Deployment Cycles**: Codebase gets large, leading to slower build and deploy cycles.
3. **Technology Lock-in**: Difficult to adopt new technologies or frameworks as the entire system is tightly coupled.

### Microservices Architecture

### Advantages:

1. **High Scalability**: Easier to scale individual services independently based on demand.
2. **Tech Stack Flexibility**: Each service can have its own technology stack, enabling the best tool for each service's needs.
3. **Resilience**: Failure in one service doesn't mean the entire system goes down.

### Downsides:

1. **Operational Complexity**: Requires sophisticated CI/CD pipelines, monitoring, and logging.
2. **Data Consistency**: CAP theorem limitations and eventual consistency can be issues.
3. **Service Communication**: Network latency and fault tolerance become concerns.

### Service Registry & Discovery

### What's Service Registry?

A service registry is a centralized database where services can register themselves and discover other services.

### Tools for Service Discovery

- **Consul**: Provides service discovery, along with health checking and a globally distributed key-value store.
- **Etcd**: A reliable key-value store for distributed systems.
- **Zookeeper**: Used for maintaining configuration information and providing distributed synchronization.

### Where Do We Need Them?

Primarily in microservices architectures for dynamic service discovery, configuration, and distributed system coordination.

### Load-Balancing

### Application Requirements:

- **High Availability**
- **Scalability**
- **Redundancy**

### What's HA (High Availability)?

A system design approach to ensure that a prearranged level of operational performance will be met during a contractual measurement period.

### What's Replication?

The act of duplicating data from one database server to another.

### What's Sharding?

Splitting a large database into smaller, more manageable pieces, or shards.

### Scaling

### Horizontal Scaling

Adding more nodes to a system.

### Vertical Scaling

Increasing the resources of a single node (e.g., CPU, RAM).

### Distributed Transactions

### What's SAGA?

A Saga is a sequence of local transactions. If one transaction fails, the Saga executes compensating transactions to undo the impact.

### What's Two-Phase Commit?

A distributed transaction protocol where a coordinator node controls the commit or rollback of transactions across multiple databases.

### Metrics, Monitoring, Tracing, Logging

### What's CorrelationId?

A unique identifier that tracks a request as it traverses multiple services in a distributed system.

### What's Distributed Tracing?

Monitoring a request as it moves through a distributed system.

### What are Metrics?

Quantifiable measures used to track system performance.

### What's Monitoring?

Continuous observation of a system to ensure it meets performance criteria.

### What's Centralized Logging?

Logging where data is sent to a central server for analysis.

### What's ELK?

Stands for Elasticsearch (search and analytics engine), Logstash (server-side data processing pipeline), and Kibana (visualizes data).

### How to Keep Logs While the Logging Provider Is Down?

Buffer logs locally and then transmit them when the service is back up.

### Key-Vaults

### Where to Store Secret Things?

In secure, encrypted storage like AWS Secrets Manager, Azure Key Vault, or HashiCorp Vault.

### What's Key-Vault?

A secure data store for sensitive information like passwords, encryption keys, and certificates.

### Service-Mesh

### What's Service-Mesh?

A dedicated infrastructure layer for facilitating service-to-service communication.

### What's Side-Car Pattern?

A single-node pattern that allows responsibilities to be abstracted away from the main application to a secondary utility.

### Communication Patterns

- **Inbox/Outbox**: Message queues for each service.
- **Fan-in/Fan-Out**: Aggregating multiple messages from one queue to another.
- **Pub/Sub**: Publish/Subscribe pattern for message exchange.
- **Peer-2-Peer**: Direct communication between each service.

### How Microservices Can Talk to Each Other?

Via HTTP/REST, message queues, gRPC, etc.

### What's gRPC? What's Protobuf?

gRPC is a high-performance, universal RPC framework. Protobuf is a binary serialization format used by gRPC.

### Message Delivery Semantics

### What's At-Least-Once?

Messages are delivered at least once, but duplicates can occur.

### What's At-Most-Once?

Messages are delivered at most once, and delivery is not guaranteed.

### How to Achieve Exactly-Once?

By using a combination of message deduplication, idempotent processing, and transactions.

### What to Do When a Message Doesn't Get Delivered?

Use a Dead Letter Queue or apply a Retry pattern.

### What's Retry Pattern?

A software pattern that re-attempts a failed operation a predetermined number of times before giving up.

I hope this deep dive provides you with the insights you were looking for. If you have more questions or need further clarification, feel free to ask.
