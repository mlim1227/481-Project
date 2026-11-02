# Solitaire Solver: Comparing Search Algorithms for Automated Solitaire

A CPSC 481 Artificial Intelligence group project exploring **Breadth-First Search (BFS)**, **Depth-First Search (DFS)**, **A\***, and optionally **Greedy Best-First Search** in a Python implementation of Solitaire.

> **Status: Repository scaffold only.** The game, graphical interface, and search algorithms are not implemented yet. This starter package establishes the folder structure for the team.

## Project goals

- Build a playable Solitaire game using Python and pygame.
- Represent game states and generate legal moves with reusable game logic.
- Implement search algorithms using the same game rules and test states.
- Compare performance using games solved, solution length, states explored, and runtime.

## Folder guide

| Path | Purpose |
| --- | --- |
| `main.py` | Application entry point (currently a placeholder) |
| `solitaire/cards.py` | Cards, suits, and deck representation |
| `solitaire/state.py` | Immutable or copyable Solitaire game-state representation |
| `solitaire/rules.py` | Legal move generation and application |
| `solitaire/game.py` | Game setup, progress, and win detection |
| `solitaire/gui.py` | pygame presentation and user interaction |
| `solitaire/solvers/` | BFS, DFS, A*, and optional Greedy algorithms |
| `assets/cards/` | Card artwork or other graphics |
| `tests/` | pytest tests |
| `results/` | Benchmark script and experiment data |
| `docs/` | Architecture notes and final-report outline |

## Setup and running

See [`README.txt`](README.txt) for installation steps and the exact commands. For now, `python main.py` prints a scaffold-only notice; it does **not** start a playable game.

## Team workflow

Develop new features on branches, open pull requests for review, and avoid merging untested changes directly to `main`.

## Key decision still open

The team has not yet decided whether search will use complete information or partial information with replanning. Keep game state and move logic separate from the GUI so either approach can be supported later.
