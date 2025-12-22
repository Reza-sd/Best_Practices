

###  mistakes in system design

 Here are the biggest mistakes I see 99% of YOU making in system design interviews:

- Jumping into design without clarifying requirements

- Spending too much time on requirements analysis (and running out of time)

- Not defining the scope and priorities (and end up designing everything... badly)

- Failing to state assumptions (scale, traffic, SLA, and so on)

- Ignoring scalability and future growth (designing for 10 users instead of 1 million)

- Overlooking performance and latency

- Forgetting fault tolerance and single points of failure

- Skipping security and privacy concerns

- Treating observability as a “bonus” instead of a requirement

- Lacking a structured approach (by not doing enough mock interviews)

- Diving into details before giving a high-level overview

- Not breaking the system into modular components

- Staying surface-level without enough technical depth

- Skipping data modeling

- Choosing improper databases

- Not accounting for data growth (no sharding/partitioning)

- Misusing or ignoring caching

- Over-engineering or under-engineering the solution

- Neglecting to discuss trade-offs while giving answers

- Failing to consider alternative solutions

- Using generic BUZZWORDS without specifics

- Lacking depth in key concepts

- Not explaining your thought process (thinking silently)

- Monologuing without engaging the interviewer

- Ignoring interviewer’s feedback or hints

- Poor time management and pacing

- Getting lost in one detail (and never coming back)

- Using a one-size-fits-all template solution

- Leaving out critical architectural components

- Failing to address edge cases and extreme scenarios

- Ignoring consistency vs availability trade-off (CAP theorem)

- Skipping back-of-the-envelope calculations

- Overlooking cost implications

- Focusing on irrelevant failure modes (while ignoring core ones)

- Bluffing when you don’t know (and getting exposed instantly)

- Not validating your design against requirements

- Neglecting to use a clear diagram or visual aid

- Not summarizing your solution at the end

- Being “passive” and waiting for the interviewer to lead

- Never walking through an actual user scenario (start to finish)

- Treating the interview like a quiz instead of a collaborative discussion
- ----------------------------------------------------
39 mistakes YOU make in scaling a
system
NEO KIM

Here are the biggest mistakes I see 99% of YOU making in scaling a system:
1. Scaling vertically instead of horizontally (and hitting hard limits)
2. Adding “microservices” too early (plus unnecessary complexity)
3. Ignoring load balancing
4. Not using caching at all… and increasing system load linearly with traffic
5. Caching ‘everything’ blindly (causing stale data, memory pressure,
complexity)
6. Forgetting CDNs for static assets
7. Keeping the server STATEFUL… (and limiting horizontal scalability +
recovery)
8. Scaling compute before data (databases are usually the first bottleneck)
9. Treating the database as “infinite” storage
10. Not using read replicas
11. Sharding BEFORE understanding access patterns
12. Never indexing ‘critical’ queries
13. Allowing SLOW queries reach production… and amplify under load
14. Blocking requests with “synchronous” processing
15. Not using QUEUES for background jobs

16. Ignoring retries and back-off… transient failures are typical in distributed
systems
17. Not setting “timeouts” (and causing thread exhaustion + cascading
failures)
18. Forgetting RATE LIMITS
19. Letting failures ‘cascade’ by not using circuit breakers
20. Ignoring backpressure
21. Deploying ONLY to a single zone/region (and failing during zone/region
outages)
22. No global traffic routing
23. Manual scaling instead of auto scaling (and moving slowly on traffic
spikes)
24. Shipping without ‘load testing’
25. Never doing “capacity planning”
26. Storing big files in databases (instead of object storage)
27. Sending uncompressed payloads
28. Making “excessive“ network calls
29. Not BATCHING for writes
30. No ‘service discovery’
31. No failover strategy
32. No graceful degradation… and disrupting core functionality under load
33. Retries without ‘idempotency’ (and causing data corruption)
34. No observability,,, you cannot scale what you cannot measure
35. No monitoring alerts
36. No “tracing” across services in a distributed system
37. Scaling features instead of fixing BOTTLENECKS
38. ‘Blindly’ copying big tech architectures
39. Believing scale is about tools,,, not tradeoffs
