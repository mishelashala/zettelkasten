#DatabaseReplication 

## Multi-master replication

"Instead of increasing the next ID by 1, we increase it by k, where k is the number of database servers in use."

Alex Xu, System Design Interview

### Multi-master replication: drawbacks

- Hard tto scale with multiple data centers
- IDs do not go up with time accross mutiple servers
- It does not scale well when a server is added or removed

Alex Xu, System Design Interview