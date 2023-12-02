# Fixed window counter algorithm
* id: f_k-XoKKp7X9V2WE5I_km
* parents: [[Popular algorithms for rate limiting]]

"Fixed window counter algorithm works as follows:
- The algorithm divides the timeline into fix-sized time windows and assign a counter for each window.
- Each request increments the counter by one.
- Once the counter reaches the pre-defined threshold, new requests are dropped until a new time window starts."

Alex Xu, System Design Interview