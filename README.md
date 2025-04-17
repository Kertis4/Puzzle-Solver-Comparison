# Puzzle Solver Search Comparison

This project implements and compares two classic search algorithms — Breadth-First Search (BFS) and Best-First Search (BestFS) — for solving sliding tile puzzles (e.g., 3x3). It evaluates their performance through simulations and visualizes results using histograms.

## Overview

The puzzle modeled here is based on the classic 8-puzzle. A board is randomly shuffled, and the solver attempts to return it to the goal state using one of the two algorithms.

The program performs multiple simulations and tracks:
- Execution time for each algorithm
- Number of moves required to solve
- Success rate (whether a solution was found)
- Distribution of outcomes via histograms

## Algorithms

### Breadth-First Search (BFS)
- Explores all paths at the same depth before moving deeper.
- Guarantees the shortest solution path.
- Can be slow or memory-intensive for large boards.

### Best-First Search (BestFS)
- Prioritizes states based on their similarity to the goal.
- Often faster but does not guarantee the shortest path.
- Heuristic used: number of correctly placed tiles.

## Features

- Adjustable puzzle size (default: 3x3)
- Adjustable shuffle depth to vary puzzle complexity
- Configurable number of simulation runs (default: 1000)
- Performance tracking (time and move count)
- Histograms to compare algorithm performance

## Requirements

- Python 3.x
- `matplotlib` for plotting

Install dependencies using:

```bash
pip install matplotlib
