# W3D5 — the benchmark harness

## Objective

The goal of this lab was to run the given benchmark harness against my locked model, sweep concurrency, find the knee where p95 crosses my target while throughput flattens, and write the one-page capacity note. Publish tokens/s and p95 to the progress board.

## Predict
- As concurrency rises, throughput (tokens/s) climbs, then flattens; p95 latency is flat at low concurrency, then climbs. Your knee (where p95 crosses target as throughput stops rising) will be at about concurrency **16**.
- Pick a target: p95 end-to-end latency of **2.0** seconds. This is your SLO for today.
