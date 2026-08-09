# VASP Performance Engine - 514K checks/sec + O(1) Compliance

High-performance VASP compliance engine for Hong Kong SFC Travel Rule.

![Architecture](docs/architecture.png)

## Benchmark
- Throughput: 514,463 checks/sec
- Architecture: Direct O(1) hash lookup - unordered_set
- Blacklist: 5,000 entries
- Compliance: SFC Travel Rule HKD 8000
- Target: OSL | HashKey - Staff Engineer
- Build: C++17 -O3 + pybind11

See Flexibility counterpart: https://github.com/nsmanju/vasp-flexibility-engine
