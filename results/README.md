# Computational results

This directory contains per-instance results for the computational comparisons in the manuscript and supplementary experiments.

| File | Contents |
| --- | --- |
| `table2_ti_fl_cp_instance_results.csv` | TI, FL, and CP formulations (Table 2; 180 instances per method) |
| `table3_cp_cpvis_lbbdv4_instance_results.csv` | CP, CP+VIs, and LBBD-v4 (Table 3; 1,800 instances per method) |
| `lbbd_variants_instance_results.csv` | LBBD-v1 through LBBD-v4 (Appendix F; 900 instances per method) |
| `benders_cuts_instance_results.csv` | LBBD-v1, LBBD-v1+RBC, and LBBD-v1+SBC (720 instances per method) |
| `lbbd_v4_instance_results.csv` | LBBD-v4 results for all 1,800 instances |
| `lbbd_v4_summary.csv` | Aggregated LBBD-v4 statistics |

## Objective scale

Objective values and bounds are scenario sums. Divide by the number of scenarios to obtain the SAA average.

## Column definitions

- `instance_path`: Relative path to the benchmark instance.
- `method`: Solution method.
- `tasks`, `machines`, `scenarios`: Numbers of tasks, machines, and scenarios.
- `psc`: Precedence-structure complexity (`L` or `H`).
- `instance_index`: Instance index within the parameter combination.
- `solve_time_seconds`: Reported computational time, in seconds.
- `lower_bound`, `upper_bound`: Objective lower and upper bounds.
- `gap_percent`: Optimality gap, calculated as `100 * (upper_bound - lower_bound) / upper_bound`.
- `optimal`: Indicator of proven optimality (1 if optimal, 0 otherwise).
- `iterations`: Number of callback iterations.
- `cut_count`: Total number of generated cuts.
- `subproblem_time_seconds`: Cumulative time attributed to subproblem processing and cut generation, in seconds.
