# W3D5 — the benchmark harness

## Objective

The goal of this lab was to run the given benchmark harness against my locked model, sweep concurrency, find the knee where p95 crosses my target while throughput flattens, and write the one-page capacity note. Publish tokens/s and p95 to the progress board.

## Predict
- As concurrency rises, throughput (tokens/s) climbs, then flattens; p95 latency is flat at low concurrency, then climbs. Your knee (where p95 crosses target as throughput stops rising) will be at about concurrency **16**.
- Pick a target: p95 end-to-end latency of **2.0** seconds. This is your SLO for today.
- 
## Publish Benchmark Results

For this run:

- **Model:** `Qwen/Qwen2.5-1.5B-Instruct-AWQ`
- **Knee concurrency:** `8`
- **Tokens/s at knee:** `487.53`
- **p95 latency at knee:** `1.8443 s`
- **Errors:** `0`

## Verification step:
levels: 5, concurrencies: [1, 2, 4, 8, 16], total errors: 0
capacity-note.md: all fields filled
GREEN CHECK: PASS
