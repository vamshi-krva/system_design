This repository contains free resources to learn System Design concepts and prepare for interviews.

80% of the System Design interviews I’ve given in the last 7 years…
…have revolved around just 20% of the most repeated, practical problems.

If you’re preparing for FAANG+ interviews or just trying to learn System Design the right way, this is the MUST-SOLVE LIST.

I've categorized them based on themes + added notes on what each one really tests you on.

► Read-Heavy Systems  
These focus on scale, latency, and efficient data fetching.  
1. Design a URL Shortener (Bitly)  
   → Talk about key generation, collisions, and DB storage.  
   → Add caching and DB sharding if traffic is high.

2. Design an Image Hosting Service  
   → Talk about object storage (S3, GCS) + CDN usage.  
   → Consider image deduplication and resizing strategies.

3. Design a Social Media Platform (Twitter/Facebook)  
   → Talk about posts, timelines, relationships (follows, friends).  
   → Focus on denormalized storage and sharding.

4. Design a NewsFeed System (Hard)  
   → Push vs Pull models, Fanout on Write vs Read.  
   → Caching, pagination, and ranking algorithms.

► Write-Heavy Systems  
Here, durability, throughput, and ingestion speed are critical.

5. Design a Rate Limiter  
   → Token bucket or leaky bucket algorithms.  
   → Redis-backed counters + TTL logic.

6. Design a Log Collection and Analysis System  
   → Use Kafka for ingestion, and something like ELK for processing.  
   → Talk about partitioning, buffering, and real-time querying.

7. Design a Voting System  
   → Idempotency, fraud prevention, and result aggregation.  
   → Real-time vs eventual vote count updates.

8. Design a Trending Topics System  
   → Use count-min sketch or approximate counting.  
   → Talk about sliding window aggregation + ranking.

► Strong Consistency Systems  
Transactional integrity and failure handling become the focus.

9. Design an Online Ticket Booking System  
   → Handle race conditions with locking or optimistic concurrency.  
   → Talk about seat reservation + payment flow.

10. Design an E-Commerce Website (Amazon)  
   → Cover product catalog, cart service, order processing.  
   → Include DB consistency, checkout idempotency.

11. Design an Online Messaging App (WhatsApp/Slack)  
   → Talk about message queues, delivery receipts, retries.  
   → Offline storage, notification delivery, scaling chat infra.

12. Design a Task Management Tool  
   → CRUD APIs, user auth, task assignment.  
   → Background jobs, status updates, and audit trails.

► Scheduler Services  
Timing, reliability, and eventual execution are tested here.

13. Design a Web Crawler  
   → BFS vs DFS for crawling, politeness rules.  
   → Distributed queues, duplicate URL filters.

14. Design a Task Scheduler  
   → Job queues, retry logic, cron-based triggers.  
   → Priority queues and task deduplication.

15. Design a Real-Time Notification System  
   → Push vs Polling, webhooks, and device token mgmt.  
   → Scale delivery across millions of users.



Namaste JavaScript by Akshay Saini 🚀:
 - https://lnkd.in/gYVUUp25

LLD by Shrayansh Jain:
 - https://lnkd.in/gFxtSxJU

HLD by Shrayansh Jain:
 - https://lnkd.in/gtgR2FEQ

System Design by Gaurav Sen:
 - https://lnkd.in/gF8Q4mef

Designing Microservices by Arpit Bhayani:
 - https://lnkd.in/gebTXbDC

Frontend Machine Coding by Piyush Agarwal:
 - https://lnkd.in/gexXg8eG

Frontend System Design by Piyush Agarwal:
 - https://lnkd.in/g3C6C3eM

SQL by Ankit Bansal:
 - https://lnkd.in/gEK8KKC5

Java by Shrayansh Jain:
 - https://lnkd.in/g2qhipNK

Spring Boot by Shrayansh Jain:
 - https://lnkd.in/gaDXrjTc

A2Z DSA sheet by Raj Vikramaditya:
 - https://lnkd.in/dQMGy9zF

𝗞𝗲𝗲𝗽𝗶𝗻𝗴 𝘁𝗵𝗶𝘀 𝗶𝗻 𝗺𝗶𝗻𝗱, 𝗜’𝘃𝗲 𝗽𝗿𝗲𝗽𝗮𝗿𝗲𝗱 𝗶𝗻 𝗗𝗲𝗽𝘁𝗵 𝗦𝘆𝘀𝘁𝗲𝗺 𝗗𝗲𝘀𝗶𝗴𝗻 𝗚𝘂𝗶𝗱𝗲.

𝗚𝗲𝘁 𝘁𝗵𝗲 𝗚𝘂𝗶𝗱𝗲 𝗵𝗲𝗿𝗲: 
 - https://lnkd.in/dte69Z5N




1. Security: Protect Your Systems
A secure system is non-negotiable. Learn:

 ✔ Authentication & Authorization (OAuth 2.0, JWT)
 
 ✔ Encryption & Cryptography (AES, RSA)
 
 ✔ OWASP Top 10 (Common security risks & how to prevent them)
 
 ✔ Threat Detection (SEIM, IDS, IPS)

2. Performance: Make It Lightning Fast 
Every millisecond counts. Optimize with:

 ✔ Caching Strategies (Redis, Memcached)
 ✔ Rate Limiting & Throttling (Prevent abuse & overload)
 ✔ Load Balancing (Distribute traffic efficiently)
 ✔ Chaos Engineering (Test system resilience)
 ✔ Fault Tolerance (Recover from failures gracefully)

3, Database Engineering: Query 
Backend engineers who understand databases deeply have a huge advantage:

 ✔ Query Optimization & Indexing (Faster queries, better performance)
 ✔ Database Trade-offs (SQL vs NoSQL)
 ✔ Transactions & Isolation Levels (ACID principles)
 ✔ Sharding & Partitioning (Scaling databases effectively)

4. API Design: Build APIs Developers Love 
Design APIs that are scalable, maintainable, and easy to use:

 ✔ OpenAPI 3.0 (Industry-standard API documentation)
 ✔ REST vs GraphQL (Choosing the right approach)
 ✔ Status Codes, Versioning & Pagination (Best practices)

6. Architecture & Paradigms: Choose the Right Structure 
The right architecture makes or breaks a system:

 ✔ Monolith vs Microservices vs Modular Monolith
 ✔ Serverless vs Traditional Backend
 ✔ Concurrency, Parallelism & Multithreading
 ✔ Optimistic vs Pessimistic Locking (Handling data consistency)

8. Distributed Systems: Scaling
Modern backend systems are distributed. Learn:

 ✔ Microservices Patterns (SAGA, CQRS, Event Sourcing)
 ✔ Event-Driven Architecture (Kafka, RabbitMQ)
 ✔ gRPC & Protobuf (Faster, efficient communication)

9. DevOps: Deploy & Manage Systems
Being DevOps-aware helps backend engineers build better software:

 ✔ CI/CD Pipelines (Automate deployments)
 ✔ Containerization (Docker, Kubernetes)
 ✔ Understanding SLAs & Incident Management

10. Observability: Know What's Happening in Your System

✔ Logging, Monitoring & Tracing (ELK, Prometheus, Jaeger)
 ✔ Performance Profiling & Optimization
 ✔ Alerting & Incident Response

Mastering these areas will elevate you from just writing APIs to designing scalable, secure, and high-performance backend systems.


1. Latency vs Throughput: https://lnkd.in/gSBsmijw
2. CAP Theorem: https://lnkd.in/gV7NunUD
3. ACID Transactions: https://lnkd.in/gpQMxV9u
4. Consistent Hashing: https://lnkd.in/gaCVWBJM
5. Rate Limiting: https://lnkd.in/gjkrHkGu
6. Microservices Architecture: https://lnkd.in/gy3kRzep
7. API Design: https://lnkd.in/ghcbQySg
8. Strong vs Eventual Consistency: https://lnkd.in/g2ACr56Q
9. Synchronous vs asynchronous communications: https://lnkd.in/gYZ8Acth
10. REST vs RPC: https://lnkd.in/gs7htCMG
11. Batch Processing vs Stream Processing: https://lnkd.in/gBKHzqAe
12. Fault Tolerance: https://lnkd.in/ggzdZVhM
13. Consensus Algorithms: https://lnkd.in/gUcVEhUx
14. Gossip Protocol: https://lnkd.in/gvkckQGY
15. Serverless Architecture: https://lnkd.in/g3EYA3nz
16. Service Discovery: https://lnkd.in/gt84khQG
17. Disaster Recovery: https://lnkd.in/grpEFGfD
18. Distributed Tracing: https://lnkd.in/ga5FJuH2
19. Horizontal vs Vertical Scaling: https://lnkd.in/eQc9FRjf
20. Content Delivery Network (CDN): https://lnkd.in/e7reQ4VF
21. Domain Name System (DNS): https://lnkd.in/es8Fp7Q5
22. Caching: https://lnkd.in/eZkyjptm
23. Distributed Caching: https://lnkd.in/e4AHNSeT
24. Load Balancing: https://lnkd.in/eWdwhGap
25. SQL vs NoSQL: https://lnkd.in/es6vJwit
26. Database Index: https://lnkd.in/ebKcznNJ
27. Consistency Patterns: https://lnkd.in/eTZ5dHQx
28. HeartBeat: https://lnkd.in/eRBRtfk9
29. Circuit Breaker: https://lnkd.in/eStETWQA
30. Idempotency: https://lnkd.in/eSYjuq-b
31. Database Scaling: https://lnkd.in/egFC33Zk
32. Data Replication: https://lnkd.in/ehZjnuWx
33. Data Redundancy: https://lnkd.in/eUCxcXr2
34. Database Sharding: https://lnkd.in/eF_2KNKT
35. Microservices Guidelines: https://lnkd.in/ea8hcbqp
36. Failover: https://lnkd.in/eftew-CE
37. Proxy Server: https://lnkd.in/eVCYxMZQ
38. Message Queues: https://lnkd.in/eVeVWT3a
39. WebSockets: https://lnkd.in/eA4zYkjF
40. Bloom Filters: https://lnkd.in/eG3xPV-x
41. API Gateway: https://lnkd.in/e-zCR3ft
42. Distributed Locking: https://lnkd.in/eXsuuthN
43. Checksum: https://lnkd.in/ed4j8cfk



## 📌 System Design Key Concepts
- [Scalability](https://blog.algomaster.io/p/scalability)
- [Availability](https://blog.algomaster.io/p/system-design-what-is-availability)
- [CAP Theorem](https://blog.algomaster.io/p/cap-theorem-explained)
- [ACID Transactions](https://blog.algomaster.io/p/what-are-acid-transactions-in-databases)
- [Consistent Hashing](https://blog.algomaster.io/p/consistent-hashing-explained)
- [Rate Limiting](https://blog.algomaster.io/p/rate-limiting-algorithms-explained-with-code)
- [SPOF](https://blog.algomaster.io/p/system-design-how-to-avoid-single-point-of-failures)
- [Fault Tolerance](https://www.cockroachlabs.com/blog/what-is-fault-tolerance/)
- [Consensus Algorithms](https://medium.com/@sourabhatta1819/consensus-in-distributed-system-ac79f8ba2b8c)
- [Gossip Protocol](http://highscalability.com/blog/2023/7/16/gossip-protocol-explained.html)
- [Service Discovery](https://blog.algomaster.io/p/service-discovery-in-distributed-systems)
- [API Design](https://abdulrwahab.medium.com/api-architecture-best-practices-for-designing-rest-apis-bf907025f5f)
- [Disaster Recovery](https://cloud.google.com/learn/what-is-disaster-recovery)
- [Distributed Tracing](https://www.dynatrace.com/news/blog/what-is-distributed-tracing/)

## 🛠️ System Design Building Blocks
- [APIs](https://blog.algomaster.io/p/whats-an-api)
- [Content Delivery Network (CDN)](https://blog.algomaster.io/p/content-delivery-networks)
- [Proxy vs Reverse Proxy](https://blog.algomaster.io/p/proxy-vs-reverse-proxy-explained)
- [Domain Name System (DNS)](https://www.cloudflare.com/learning/dns/what-is-dns/)
- [Caching](https://blog.algomaster.io/p/4d7d6f8a-6803-4c7b-85ca-864c87c2cbf2)
- [Caching Strategies](https://blog.algomaster.io/p/top-5-caching-strategies-explained)
- [Distributed Caching](https://blog.algomaster.io/p/distributed-caching)
- [API Gateway](https://blog.algomaster.io/p/what-is-an-api-gateway)
- [Load Balancing](https://blog.algomaster.io/p/load-balancing-algorithms-explained-with-code)
- [Databases Types](https://blog.algomaster.io/p/15-types-of-databases)
- [SQL vs NoSQL](https://blog.algomaster.io/p/sql-vs-nosql-7-key-differences)
- [Database Indexes](https://blog.algomaster.io/p/a-detailed-guide-on-database-indexes)
- [Consistency Patterns](https://systemdesign.one/consistency-patterns/)
- [HeartBeats](https://blog.algomaster.io/p/heartbeats-in-distributed-systems)
- [Circuit Breaker](https://medium.com/geekculture/design-patterns-for-microservices-circuit-breaker-pattern-276249ffab33)
- [Idempotency](https://blog.algomaster.io/p/idempotency-in-distributed-systems)
- [Database Scaling](https://blog.algomaster.io/p/system-design-how-to-scale-a-database)
- [Data Replication](https://redis.com/blog/what-is-data-replication/)
- [Data Redundancy](https://blog.algomaster.io/p/489440f1-9c80-4241-9ec8-de156964c3b9)
- [Database Sharding](https://blog.algomaster.io/p/what-is-database-sharding)
- [Database Architectures](https://www.mongodb.com/developer/products/mongodb/active-active-application-architectures/)
- [Failover](https://www.druva.com/glossary/what-is-a-failover-definition-and-related-faqs)
- [Bloom Filters](https://blog.algomaster.io/p/bloom-filters)
- [Message Queues](https://blog.algomaster.io/p/message-queues)
- [WebSockets](https://blog.algomaster.io/p/websockets)
- [Checksums](https://blog.algomaster.io/p/what-are-checksums)
- [Microservices Guidelines](https://newsletter.systemdesign.one/p/netflix-microservices) 
- [Distributed Locking](https://martin.kleppmann.com/2016/02/08/how-to-do-distributed-locking.html)

## ⚖️ System Design Tradeoffs
- [Top 15 Tradeoffs](https://blog.algomaster.io/p/system-design-top-15-trade-offs)
- [Vertical vs Horizontal Scaling](https://blog.algomaster.io/p/system-design-vertical-vs-horizontal-scaling)
- [Concurrency vs Parallelism](https://blog.algomaster.io/p/concurrency-vs-parallelism)
- [Long Polling vs WebSockets](https://blog.algomaster.io/p/long-polling-vs-websockets)
- [Batch vs Stream Processing](https://blog.algomaster.io/p/batch-processing-vs-stream-processing)
- [Stateful vs Stateless Design](https://blog.algomaster.io/p/741dff8e-10ea-413e-8dd2-be57434917d2)
- [Strong vs Eventual Consistency](https://blog.algomaster.io/p/7d9da525-fe25-4e16-94e8-8056e7c57934)
- [Read-Through vs Write-Through Cache](https://blog.algomaster.io/p/59cae60d-9717-4e20-a59e-759e370db4e5)
- [Push vs Pull Architecture](https://blog.algomaster.io/p/af5fe2fe-9a4f-4708-af43-184945a243af)
- [REST vs RPC](https://blog.algomaster.io/p/106604fb-b746-41de-88fb-60e932b2ff68)
- [Synchronous vs. asynchronous communications](https://blog.algomaster.io/p/aec1cebf-6060-45a7-8e00-47364ca70761)
- [Latency vs Throughput](https://aws.amazon.com/compare/the-difference-between-throughput-and-latency/)

## 🖇️ System Design Architectural Patterns
- [Client-Server Architecture](https://blog.algomaster.io/p/4585cf8e-30a4-4295-936f-308a25cb716c)
- [Microservices Architecture](https://medium.com/hashmapinc/the-what-why-and-how-of-a-microservices-architecture-4179579423a9)
- [Serverless Architecture](https://blog.algomaster.io/p/2edeb23b-cfa5-4b24-845e-3f6f7a39d162)
- [Event-Driven Architecture](https://www.confluent.io/learn/event-driven-architecture/)
- [Peer-to-Peer (P2P) Architecture](https://www.spiceworks.com/tech/networking/articles/what-is-peer-to-peer/)

## ✅ How to Answer a System Design Interview Problem
<img src="diagrams/interview-template.png" width="400" height="250">

### [Read the Full Article](https://blog.algomaster.io/p/how-to-answer-a-system-design-interview-problem)

## 💻 System Design Interview Problems
### Easy
- [Design URL Shortener like TinyURL](https://blog.algomaster.io/p/design-a-url-shortener)
- [Design Text Storage Service like Pastebin](https://www.youtube.com/watch?v=josjRSBqEBI)
- [Design Leaderboard](https://systemdesign.one/leaderboard-system-design/)
- [Design Content Delivery Network (CDN)](https://www.youtube.com/watch?v=8zX0rue2Hic)
- [Design Parking Garage](https://www.youtube.com/watch?v=NtMvNh0WFVM)
- [Design Vending Machine](https://www.youtube.com/watch?v=D0kDMUgo27c)
- [Design Distributed Key-Value Store](https://www.youtube.com/watch?v=rnZmdmlR-2M)
- [Design Distributed Cache](https://www.youtube.com/watch?v=iuqZvajTOyA)
- [Design Authentication System](https://www.youtube.com/watch?v=uj_4vxm9u90)
- [Design Unified Payments Interface (UPI)](https://www.youtube.com/watch?v=QpLy0_c_RXk)
### Medium
- [Design WhatsApp](https://blog.algomaster.io/p/design-a-chat-application-like-whatsapp)
- [Design Spotify](https://blog.algomaster.io/p/design-spotify-system-design-interview)
- [Design Distributed Job Scheduler](https://blog.algomaster.io/p/design-a-distributed-job-scheduler)
- [Design a Scalable Notification Service](https://blog.algomaster.io/p/design-a-scalable-notification-service)
- [Design Instagram](https://www.youtube.com/watch?v=VJpfO6KdyWE)
- [Design Tinder](https://www.youtube.com/watch?v=tndzLznxq40)
- [Design Facebook](https://www.youtube.com/watch?v=9-hjBGxuiEs)
- [Design Twitter](https://www.youtube.com/watch?v=wYk0xPP_P_8)
- [Design Reddit](https://www.youtube.com/watch?v=KYExYE_9nIY)
- [Design Netflix](https://www.youtube.com/watch?v=psQzyFfsUGU)
- [Design Youtube](https://www.youtube.com/watch?v=jPKTo1iGQiE)
- [Design Google Search](https://www.youtube.com/watch?v=CeGtqouT8eA)
- [Design E-commerce Store like Amazon](https://www.youtube.com/watch?v=EpASu_1dUdE)
- [Design TikTok](https://www.youtube.com/watch?v=Z-0g_aJL5Fw)
- [Design Shopify](https://www.youtube.com/watch?v=lEL4F_0J3l8)
- [Design Airbnb](https://www.youtube.com/watch?v=YyOXt2MEkv4)
- [Design Autocomplete for Search Engines](https://www.youtube.com/watch?v=us0qySiUsGU)
- [Design Rate Limiter](https://www.youtube.com/watch?v=mhUQe4BKZXs)
- [Design Distributed Message Queue like Kafka](https://www.youtube.com/watch?v=iJLL-KPqBpM)
- [Design Flight Booking System](https://www.youtube.com/watch?v=qsGcfVGvFSs)
- [Design Online Code Editor](https://www.youtube.com/watch?v=07jkn4jUtso)
- [Design Stock Exchange System](https://www.youtube.com/watch?v=dUMWMZmMsVE)
- [Design an Analytics Platform (Metrics & Logging)](https://www.youtube.com/watch?v=kIcq1_pBQSY)
- [Design Payment System](https://www.youtube.com/watch?v=olfaBgJrUBI)
- [Design a Digital Wallet](https://www.youtube.com/watch?v=4ijjIUeq6hE)
### Hard
- [Design Location Based Service like Yelp](https://www.youtube.com/watch?v=M4lR_Va97cQ)
- [Design Uber](https://www.youtube.com/watch?v=umWABit-wbk)
- [Design Food Delivery App like Doordash](https://www.youtube.com/watch?v=iRhSAR3ldTw)
- [Design Google Docs](https://www.youtube.com/watch?v=2auwirNBvGg)
- [Design Google Maps](https://www.youtube.com/watch?v=jk3yvVfNvds)
- [Design Zoom](https://www.youtube.com/watch?v=G32ThJakeHk)
- [Design Distributed Counter](https://systemdesign.one/distributed-counter-system-design/)
- [Design File Sharing System like Dropbox](https://www.youtube.com/watch?v=U0xTu6E2CT8)
- [Design Ticket Booking System like BookMyShow](https://www.youtube.com/watch?v=lBAwJgoO3Ek)
- [Design Distributed Web Crawler](https://www.youtube.com/watch?v=BKZxZwUgL3Y)
- [Design Code Deployment System](https://www.youtube.com/watch?v=q0KGYwNbf-0)
- [Design Distributed Cloud Storage like S3](https://www.youtube.com/watch?v=UmWtcgC96X8)
- [Design Distributed Locking Service](https://www.youtube.com/watch?v=v7x75aN9liM)
- [Design Slack](https://systemdesign.one/slack-architecture/)
- [Design Live Comments](https://systemdesign.one/live-comment-system-design/)

## 📚 Books
- [Designing Data-Intensive Applications](https://www.amazon.in/dp/9352135245)

## 📩 Newsletters
- [AlgoMaster Newsletter](https://blog.algomaster.io/)

## 📺 YouTube Channels
- [Tech Dummies Narendra L](https://www.youtube.com/@TechDummiesNarendraL)
- [Gaurav Sen](https://www.youtube.com/@gkcs)
- [codeKarle](https://www.youtube.com/@codeKarle)
- [ByteByteGo](https://www.youtube.com/@ByteByteGo)
- [System Design Interview](https://www.youtube.com/@SystemDesignInterview)
- [sudoCODE](https://www.youtube.com/@sudocode)
- [Success in Tech](https://www.youtube.com/@SuccessinTech/videos)

## 📜 Must-Read Engineering Articles
- [How Discord stores trillions of messages](https://discord.com/blog/how-discord-stores-trillions-of-messages)
- [Building In-Video Search at Netflix](https://netflixtechblog.com/building-in-video-search-936766f0017c)
- [How Canva scaled Media uploads from Zero to 50 Million per Day](https://www.canva.dev/blog/engineering/from-zero-to-50-million-uploads-per-day-scaling-media-at-canva/)
- [How Airbnb avoids double payments in a Distributed Payments System](https://medium.com/airbnb-engineering/avoiding-double-payments-in-a-distributed-payments-system-2981f6b070bb)
- [Stripe’s payments APIs - The first 10 years](https://stripe.com/blog/payment-api-design)
- [Real time messaging at Slack](https://slack.engineering/real-time-messaging/)

## 🗞️ Must-Read Distributed Systems Papers
- [Paxos: The Part-Time Parliament](https://lamport.azurewebsites.net/pubs/lamport-paxos.pdf)
- [MapReduce: Simplified Data Processing on Large Clusters](https://research.google.com/archive/mapreduce-osdi04.pdf)
- [The Google File System](https://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf)
- [Dynamo: Amazon’s Highly Available Key-value Store](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf)
- [Kafka: a Distributed Messaging System for Log Processing](https://notes.stephenholiday.com/Kafka.pdf)
- [Spanner: Google’s Globally-Distributed Database](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf)
- [Bigtable: A Distributed Storage System for Structured Data](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)
- [ZooKeeper: Wait-free coordination for Internet-scale systems](https://www.usenix.org/legacy/event/usenix10/tech/full_papers/Hunt.pdf)
- [The Log-Structured Merge-Tree (LSM-Tree)](https://www.cs.umb.edu/~poneil/lsmtree.pdf)
- [The Chubby lock service for loosely-coupled distributed systems](https://static.googleusercontent.com/media/research.google.com/en//archive/chubby-osdi06.pdf)

---

