#ConsistencyModels

## Strong Consistency

"any read operation returns a value corresponding to the result of the most updated write data item. A client never sees out-of-date-data."

Alex Xu, System Design Interview

### How strong consistency is achieved

"Strong consistency is usually achieved by forcing a replica not to accept new reads/writes until every replica has agreed on current write."

Alex Xu, System Design Interview

---

## Weak Consistency

"subsequent read operations may not seed the most updated value."

Alex Xu, System Design Interview

### Inconsistent resolution versioning

"Replication gives high availability but causes inconsistencies among replicas. Versioning and vector locks are used to solve inconsistency problems."

Alex Xu, System Design Interview

---

## Eventual consistency

"This is a specific form of weak consistency. Given anough time, all updates are propagated, and all replicas are consistent."

Alex Xu, System Design Interview