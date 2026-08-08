# VASP Performance Engine - 514K checks/sec ⚡

High-performance VASP compliance screening - Direct call O(1) hash.

## Benchmark
| Metric | Value |
|--------|-------|
| Throughput | **514,463 checks/sec** |
| Data Structure | `unordered_set` O(1) |
| Blacklist | 5,000 entries (17 real + 4982 synthetic + 1 BTC) |
| Build | C++17 -O3 + pybind11 |
| Compliance | SFC Travel Rule HKD 8000 |

## Architecture
- Direct inline hash lookup - minimal overhead
- No virtual dispatch
- Best for: Maximum throughput, low-latency

## Build
```bash
make clean && make && make test
