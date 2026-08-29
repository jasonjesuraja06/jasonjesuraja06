Third-year CS student at Georgia Tech. I build systems software and measure it honestly.

### Projects

**[clockwork](https://github.com/jasonjesuraja06/clockwork)** - LLM inference engine for agent workloads. Continuous batching, a paged KV cache with copy-on-write, a radix-tree prefix cache, and a Triton paged-attention kernel behind an OpenAI-compatible API. Greedy decoding is token-exact against the Hugging Face reference, enforced in CI. Benchmarked against vLLM on a Tesla T4; every table names its hardware and links the raw CSVs.
`Python` `PyTorch` `Triton` `FastAPI`

**[heartscreen](https://github.com/jasonjesuraja06/heartscreen)** - Arrhythmia discovery engine for wearable ECG. An 821k-parameter residual CNN in JAX/Flax scoring 0.8271 mean challenge F1 on the 8,528-record CinC 2017 set, wrapped in a screening pipeline that scans 1,961 recording-hours in 15.3 minutes and ranks candidate atrial fibrillation episodes.
`Python` `JAX` `Flax` `SciPy`

**[distributed-kv-store](https://github.com/jasonjesuraja06/distributed-kv-store)** - Raft consensus implemented from scratch in Go, with a replicated key-value store on top. Commit-before-acknowledge writes, linearizable reads through read-index, BoltDB persistence, joint-consensus membership, and a deterministic fault injector that kills leaders and partitions the network.
`Go` `gRPC` `BoltDB` `Protocol Buffers`

### How I work

Numbers in these repos come from a command that ran, recorded with the command that produced it. Where a result is unfavorable or a limitation exists, it is stated next to the number rather than omitted. Each repo ships its raw run artifacts as a release so a reader can check the tables against the data.

Reach me at [linkedin.com/in/jason-jesuraja](https://linkedin.com/in/jason-jesuraja).
