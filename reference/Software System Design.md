## Rate Limiter

"In the HTTP world, a rate limiter limits the number of client requests allowed to be sent over a specified period."

Alex Xu, System Design Interview

### High Level Architecture

"The basic idea of rate limiting algorithms is simple. At the high-level, we need a counter to keep track of how many requests are sent from the same user, IP address, etc. If the counter is larger than the limit, the request is disallowed."

Alex Xu, System Design Interview

### Benefit: Reduces costs

"Limiting excess requests means fewer servers and allocating more resources to high priority APIs."

Alex Xu, System Design Interview

### Benefit: Prevents DoS attacks

"A rate limiter prevents DoS attacks, either intentional or unintentional, by blocking the excess calls."

Alex Xu, System Design Interview

### Popular Rate Limiting Algorithms

- Token bucket
- Leaking bucket
- Fixed window counter
- Sliding window log
- Sliding window counter

Alex Xu, System Design Interview

#### Algorithm: Token Bucket

"A token bucket is a container that has pre-defined capacity. Tokens are put inn the bucket at preset rates periodically. Once the bucket is full, no more tokens can be added."

Alex Xu, System Design Interview

##### Token Bucket: Parameters

"The token bucket algorithm takes two parameters:
- Bucket size: the maximum number of tokens allowed in the bucket
- Refill rate: number of tokens put into the bucket every second"

Alex Xu, System Design Interview

##### Multiple token buckets

"It is usually necessary to have different buckets from different API endpoints."

Alex Xu, System Design Interview

#### Algorithm: Leaking bucket

"The leaking bucket algorithm is similar to the token bucket except that requests are processed at a fixed rate. It is usually implemented with a first-in-first-out (FIFO) queue."

Alex Xu, System Design Interview

##### Leaking Bucket: Parameters

"Leaking bucket algorithm takes the following two parameters:
- Bucket size: it is equal to the queue size. The queue holds the requests to be processed at a fixed rate.
- Outflow rate: it defines how many requests can be processed at a fixed rate, usually in seconds."

Alex Xu, System Design Interview

#### Algorithm: Fixed window counter

"Fixed window counter algorithm works as follows:
- The algorithm divides the timeline into fix-sized time windows and assign a counter for each window.
- Each request increments the counter by one.
- Once the counter reaches the pre-defined threshold, new requests are dropped until a new time window starts."

Alex Xu, System Design Interview

#### Algorithm: Sliding window log

"It works as follows:
- The algorithm keeps track of request timestamps. Timestamp data is usually kept in cache, such as sorted sets of Redis/
- When a new request comes in, remove all the outdated timestamps. Outedated timestamps are dfined as those older than the start of the current time window.
- Add a timestamp of the new request to the log.
- If the log size is the same or lower than the allowed count, a request is accepted. Otherwise, it is rejected."

Alex Xu, System Design Interview

#### Algorithm: Sliding window counter

"The sliding window counter algorithm is a hybrid approach that combines the fixed window counter and sliding window log."

Alex Xu, System Design Interview

### Client Side rate Limiter

"[...] client is an unreliable place to enforce rate limiting because client requests can easily be forged by malicious actors. Moreover, we might not have control over the client implementation."

Alex Xu, System Design Interview

### API gateway as rate limiter

"Cloud micro-services have become widely popular and rate limiting is usually implemented within a component called API gateway."

Alex Xu, System Design Interview

## Sharding

"Horizontal scaling, also known as sharding, is the practice of adding more servers."

Alex Xu, System Design Interview

### Shards

"Sharding separates large databases into smaller, more easily managed parts called shards."

Alex Xu, System Design Interview

### Shard Data

"Each shard shares the same schema, though the actual data on each shard is unique to the shard."

Alex Xu, System Design Interview

### Sharding Key

"Sharding key (known as a partition key) consists of one or more columns that determine how data is distributed."

Alex Xu, System Design Interview

#### Sharding Key: Usage

"A sharding key allows you to retrieve and modify data efficiently by routing database queries to the correct database."

Alex Xu, System Design Interview

### Resharding Data

"Resharding data is needed when 1) a single shard could no longer hold more data due to rapid growth. 2) Certain shards might experience shard exhaustion faster than others due to uneven data distribution."

Alex Xu, System Design Interview

### Problem: Hotspot Key

"Excessive access to a specific shard could cause server overload."

Alex Xu, System Design Interview

#### Hotspot Key Problem: Solution

"To solve this problem, we may need to allocate a shard for each celebrity [hotspot]. Each shard might even require further partition."

Alex Xu, System Design Interview

### Problem: Joins are difficult to perform

"Once a database has been sharded across multiple servers, it is hard to perform join operations across database shards."

Alex Xu, System Design Interview

#### Joins are difficult to perform: Solution

"A common workaround this us to de-normalize the database so that queries can be performed in a single table"

Alex Xu, System Design Interview

## Content Delivery Network

"A CDN is a network of geographically dispersed servers, used to deliver static content."

Alex Xu, System Design Interview

### CDN: Usage

"CDN servers cache static content like images, videos, CSS, JavaScript, files, etc."

Alex Xu, System Design Interview

### When not to use a CDN

"Cachin infrequently used assets provides no significant benefits so you should consider moving them out of the CDN."

Alex Xu, System Design Interview

### NDC Cache Expericy

"The cache expiry time should neither be too long nor too short. If it is too long, the content might no longer be fresh. If it is too short, it can cause repeat reloading of content from origin servers to the CDN."

Alex Xu, System Design Interview

### Dynamic Content Cachin

"It enables the caching of HTML pages that are based on requests path, query strings, cookies, and request headers."

Alex Xu, System Design Interview

## Cache

"A cache is a temporary storage are that stores the result of expensive responses frequently accessed data in memory so that subsequent requests are served more quickly."

Alex Xu, System Design Interview

### Benefit: Cache helps mitigate failures

"[...] multiple cache servers across different data centers are recommended to avoid SPOF [[Single Point of Failure]]"

Alex Xu, System Design Interview

### When not to use cache

"Since cached data is stored in volatile memory, a cache server is not ideal for persisting data."

Alex Xu, System Design Interview

### Cache Expiration Policy

"Once cached data is expired, it is removed from the cache. When there is no expiration policy, cached data will be stored in the memory permanently."

Alex Xu, System Design Interview

#### Cache Eviction Policy

"Once the cache is full, any request to add items to the cache might cause existing items to be removed."

Alex Xu, System Design Interview

##### Strategy: Least-recently-used

"(LRU) is the most popular cache eviction policy."

Alex Xu, System Design Interview

### Read-Through Cache

"After receiving a request, a web server first checks if the cache has the available response. If it has, it sends data back to the client. If not, it queries the database, stores the response in cache, and sends it back to the client."

Alex Xu, System Design Interview

### Cache Tier

"The cache tier is a temporary data store layer, much faster than the database."

Alex Xu, System Design Interview

### Cache Consistency

"Inconsistency can happen because data-modifying operations on the data store and cache are not in a single transaction."

Alex Xu, System Design Interview

## URL Frontier

"A URL frontier is a data structure that stores URLs to be downloaded."

Alex Xu, Design System Interview

### URL Frontier: Purpose

"The URL frontier is an important component to ensure politeness, URL prioritization, and freshness."

Alex Xu, System Design Interview

### Politeness

"Generally, a web crawler should avoid sending too many requests to the same hosting server within a short period. Sending too many requests is considered as 'impolite' or even treated as a denial-of-service (DOS) attack."

Alex Xu, System Design Interview

#### Enforcing Politeness

"The general idea of enforcing politeness is to download one page at a time from the same host. A delay can be added between two download tasks. The politeness constraint is implemented by maintain a mapping from website hostnames to download (worker) threads."

Alex Xu, System Design Interview

### Redirects

#### 301 Redirect

"A 301 redirect shows that the requested URL is 'permanently' moved to the long URL. Since it is permanently redirected, the browser caches the response, and subsequent requests for the same URL will not be sent to the URL shortening service. Instead, requests are redirected to the long URL server directly."

Alex Xu, System Design Interview

#### 302 Redirect

"A 302 redirect means that the URL is 'temporarily' moved to the long URL, meaning that subsequent requests for the same URL will be sent to the URL shortening service first. Then, they are redirected to the long URL server."

Alex Xu, System Design Interview

## geoDNS

"geoDNS is a DNS service that allows domain names to be resolved to IP addresses based on the location of a user."

Alex Xu, System Design Interview

### geoDNS outage

"In the event of any significant data center outage, we direct all traffic to a healthy data center."

Alex Xu, System Design Interview

## Load Balancer

"A load balancer evenly distributes incoming traffic among web servers that are defined in a load-balanced set."

Alex Xu, System Design Interview

### Loan Balancer and high traffic

"If the website traffic grows rapidly, and two servers are not enough to handle the traffic, the load balancer can handle this problem gracefully. You only need to add more servers to the web server pool, and the load balancer automatically starts to send requests to them."

Alex Xu, System Design Interview

### Load Balancer and app failure

"If server 1 goes offline, all the traffic will be routed to server 2. This prevents the website from going offline."

Alex Xu, System Design Interview

## CAP Theorem

"CAP theorem states it is impossible for a distributed system to simultaneously provide more than two of these three guarantees: consistency, availability, and partition tolerance."

Alex Xu, System Design Interview

### Consistency

"Consistency means all clients see the same data at the same time no matter which node they connect to."

Alex Xu, System Design Interview

### Availability

"Availability means any client which requests data gets a response even if some of the nodes are down."

Alex Xu, System Design Interview

#### High Availability

"High availability is the ability of a system to be continuously operational for a desirably long period of time."

Alex Xu, System Design Interview

#### How Availability is Measured

"High availability is measured as a percentage, with 100% means a service that has 0 downtime. Most services fall between 99% and 100%."

Alex Xu, System Design Interview

### Partition Tolerance

"A partition indicates a communication break between two nodes. Partition tolerance means the system continues to operate despite network partitions."

Alex Xu, System Design Interview

### Consistency over Availability

"If inconsistency occurs due to a network partition, [a] bank system returns an error before the inconsistency is resolved."

Alex Xu, System Design Interview

### Availability over Consistency

"If we choose availability over consistency (AP system), the system keeps accepting reads, even though it might return stale data."

Alex Xu, System Design Interview

### Distributed systems in the real world

"In a distributed system, partitions cannot be avoided ,and when a partition occurs, we must choose between consistency and availability."

Alex Xu, System Design Interview

#### Unique ID generation in Distributed Systems

"auto_increment does not work in a distributed environment because a single database server is not large enough and generating unique IDs across multiple databases with minimal delay is challenging."

Alex Xu, System Design Interview

## Scaling Strategies

### Autoscaling

"Autoscaling means adding or removing web servers automatically based on the traffic load."

Alex Xu, System Design Interview

### Vertical Scaling

"Vertical scaling, referred to as 'scale up', means the process of adding more power (CPU, RAM, etc.) to your servers."

Alex Xu, System Design Interview

#### Vertical Scaling: Disadvantage

"Vertical scaling has a hard limit. It is impossible to add unlimited CPU and memory to a single server."

Alex Xu, System Design Interview

#### Vertical Scaling: Another Disadvantage

"Vertical scaling does not have failover and redundancy. If one server goes down, the website/app goes down with it completely."

Alex Xu, System Design Interview

### Horizontal Scaling

"Horizontal scaling, referred to as 'scale-out', allows you to scale by adding more servers into your pool of resources."

Alex Xu, System Design Interview

## Fanout Service

"Fanout is the process of delivering a post to all friends."

Alex Xu, System Design Interview

### Fanout Models

"Two types of fanout models are: fanout on write (also called push model), and fanout on read (also called pull model)."

Alex Xu, System Design Interview

### Fanout on Read

"The news feed is generated during read time. This is an on-demand model. Recent posts are pulled when a user loads her home page."

Alex Xu, System Design Interview

### Fanout on Write

"With this approach, news feed is pre-computed during write time. A new post is delivered to friend's cache immediately after it is published."

Alex Xu, System Design Interview

## Ticket Server

"The idea is to user a centralized auto_increment feature in a single database server (Ticket Server)"

Alex Xu, System Design Interview

### Ticket Server and SPOF

"Single ticket server means if the ticket server goes down, all systems that depend on it will face issues. TO avoid a single point of failure, we can set up multiple ticket servers. However, this will introduce new challenges such as data synchronization."

Alex Xu, System Design Interview

### Single Point of Failure

"A single point of failure (SPOF) is a part of a system that, if it fails, will stop the entire system from working.."

Wikpedia

## Message Queue

"A message queue is a durable component, stored in memory, that supports asynchronous communication. It serves as a buffer and distributes asynchronous requests."

Alex Xu, System Design Interview

### Benefit: Message Queue Allows Decoupling

"Decoupling makes the message queue a preferred architecture for building a scalable and reliable application."

Alex Xu, System Design Interview

### When the consumer is not available

"[...] the producer can post a message to the queue when the consumer is unavailable to process it."

Alex Xu, System Design Interview

### When the producer is not available

"The consumer can read messages from the queue ven when the producer is unavailable."

Alex Xu, System Design Interview

## Bloom Filter

"A bloom filter is a space-efficient probabilistic technique to test if an element is a member of a set."

Alex Xu, System Design Interview

## Stateful Service

"The service is stateful because each client maintains a persisten network connection to a [...] server."

Alex Xu, System Design Interview

## Stateless Services

"Stateless services are traditional public-facing request/response services, used to manage the login, signup, user profile, etc."

Alex Xu, System Design Interview

## UUID

"UUID is a 128-bit number used to identify information in computer systems. UUID has a very low probability of getting [collisions]"

Alex Xu, System Design Interview

### Benefit: No need to coordinate UUID generation

"No coordination between servers is need so there will not be any synchronization issues."

Alex Xu, System Design Interview

## Private IP

"A private IP is an IP address reachable only between servers in the same network; however, it is unreachable over the internet."

Alex Xu, System Design Interview

## Consistent Hashing

"Consistent hashing is a special kind of hashing such that when a hash table is re-sized and consistent hashing is used, only k/n keys need to be remapped on average, where k is the number of keys, and n is the number of slots. In contrast, in most traditional hash tables, a change in the number of array slots causes nearly all keys to be remapped."

Wikipedia