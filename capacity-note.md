# Capacity note (team, one page)

## The numbers

- Locked model: Qwen/Qwen2.5-1.5B-Instruct-AWQ
- Target p95 end-to-end latency (your SLO today): 2.0 seconds
- Knee concurrency (highest concurrency whose p95 is still under target): 8
- Tokens per second at the knee: 487.53
- Max sustainable request rate at the target p95: 4.70 req/s

## The limiting family

- Compute-bound: throughput continues increasing strongly as concurrency rises, while p95 latency starts climbing as GPU demand increases toward saturation.

## Why the knee, not the peak

- We report concurrency 8 because it is the highest level that stays under our 2.0-second p95 SLO; concurrency 16 gives higher throughput but exceeds the latency target.