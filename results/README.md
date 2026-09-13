# LBBD-v4 results

`lbbd_v4_instance_results.csv` contains one row for each of the 1,800 released CP/LBBD comparison instances. Initial solutions and initial upper bounds are intentionally excluded.

The gap is `100 * (upper_bound - lower_bound) / upper_bound`. `solve_time_seconds` follows the manuscript reporting convention: the published 720-instance scope retains its historical wall-clock records, while the added 1,080-instance scope is capped at 3,600 seconds. Derived master-problem time fields are omitted because they cannot be consistently reconstructed from capped solve times.

`cut_count` is the solver-reported total cut count (`NtoCuts`), which is the cut metric used in the manuscript LBBD-variant figure. CP-call time, LBC timing, and the separate no-good-cut counter are omitted.

`lbbd_v4_summary.csv` reports 60 `(PSC, tasks, scenarios)` subgroups, two PSC totals, and one overall total. Each subgroup pools the three machine counts and therefore contains 30 instances. Every mean is calculated directly from the instance rows. Per-instance gap percentages are displayed to four decimals to retain small positive gaps; summary statistics are displayed to two decimals.
