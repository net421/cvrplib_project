# CVRP Optimization Framework

## Executive Summary
This project develops a hybrid optimization framework for the Capacitated Vehicle Routing Problem (CVRP), achieving ~10% optimality gap on benchmark instances.

## Business Impact
- Reduces logistics costs through improved routing efficiency
- Scalable to real-world fleet optimization problems
- Demonstrates measurable performance improvement over baseline heuristics

## Methodology
- Clarke & Wright Savings (global route construction)
- 2-opt local search (route refinement)
- Multi-instance benchmarking pipeline

## Results
| Method | GAP (%) |
|--------|--------|
| Nearest Neighbor | ~46 |
| Savings | ~27 |
| Hybrid | ~10 |

## Reproducibility
```bash
export PYTHONPATH=.
python experiments/run_benchmark.py
python experiments/plot_results.py
```

## Insight
Global structural optimization provides the largest performance gains; local refinement improves efficiency incrementally.
