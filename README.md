# RP-PMS-UPT

Benchmark instances for the resource- and precedence-constrained parallel
machine scheduling problem with uncertain processing times.

This repository contains the 1,800 stochastic instances used to compare CP,
CP+VIs, and LBBD-v4:

- tasks: 10, 15, 20, 25, and 30;
- machines: 2, 3, and 4;
- scenarios: 10, 30, 50, 100, 500, and 1,000;
- precedence-structure complexity: low (`os_0`) and high (`os_1`);
- replications: 10 for each parameter combination.

Instance filenames are normalized to `0.txt` through `9.txt`. The release
index is only an identifier and does not alter an instance. `manifest.csv`
records each public path, its dimensions, SHA-256 digest, and file size.
Sensitivity-analysis instances are not included.

The `results` directory contains the aligned LBBD-v4 per-instance results and
their aggregate summary. Initial solutions and initial upper bounds are not
included.
