# Sliding window log algorithm
* id: 4YkzqKXxXReVgl6JXsov0
* parents: [[Popular algorithms for rate limiting]]

"It works as follows:
- The algorithm keeps track of request timestamps. Timestamp data is usually kept in cache, such as sorted sets of Redis/
- When a new request comes in, remove all the outdated timestamps. Outedated timestamps are dfined as those older than the start of the current time window.
- Add a timestamp of the new request to the log.
- If the log size is the same or lower than the allowed count, a request is accepted. Otherwise, it is rejected."

Alex Xu, System Design Interview