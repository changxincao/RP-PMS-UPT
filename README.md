# RP-PMS-UPT

Benchmark instances and computational results for the resource- and precedence-constrained parallel machine scheduling problem with uncertain processing times.

## Benchmark instances

The repository provides 1,800 stochastic instances covering:

- Tasks: 10, 15, 20, 25, and 30
- Machines: 2, 3, and 4
- Scenarios: 10, 30, 50, 100, 500, and 1,000
- Precedence-structure complexity: low (`os_0`) and high (`os_1`)
- Replications: 10 per parameter combination

Each combination has ten instance files, numbered `0.txt` through `9.txt`. The `manifest.csv` file lists their paths, dimensions, SHA-256 checksums, and file sizes.

## Computational results

The `results/` directory contains per-instance computational results for:

- Time-indexed (TI), flow-based (FL), and constraint programming (CP) formulations (Table 2)
- CP, CP with valid inequalities (CP+VIs), and LBBD-v4 (Table 3)
- Four LBBD variants, LBBD-v1 through LBBD-v4 (Appendix F)
- LBBD-v1 with regular Benders cuts (RBCs) and strengthened Benders cuts (SBCs) (supplementary comparison)

An aggregate summary of LBBD-v4 results is also provided. See [results/README.md](results/README.md) for result-file descriptions and reporting conventions.
