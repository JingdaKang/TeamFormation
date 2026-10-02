# Team Formation Algorithms

C++ research implementations of expert-team formation algorithms on social networks, covering skill coverage, leader selection, capacity, online selection, and bi-objective methods.

## Requirements

A C++ toolchain plus the original graph/data support code. Sources reference headers such as `author.h`, `csv.h`, and `edges.h` that are not present in this checkout. Required graph and skill datasets are also external.

## Getting started

Read the original [algorithm and paper mapping](README). Select one implementation, obtain its missing headers and data, configure `PATH`/`SKILLPATH` and cost/capacity inputs, and check its entry point before compiling.

## Project structure

| Path | Purpose |
| --- | --- |
| `rarest_first.cpp` | Rarest-first implementation |
| `GreedyCover.cpp` | Greedy skill coverage |
| `GreedyDiameter.cpp` | Diameter-oriented selection |
| `GreedyMST.cpp` | Spanning-tree-oriented selection |
| `FindBestWO.cpp` | Team selection without a leader |
| `FindBestWLeader.cpp` | Team selection with a leader |
| `USTF_Code` | Additional algorithm variants |
| `README` | Original paper references and configuration notes |

## Configuration and limitations

Programs contain machine-specific dataset paths and some nonstandard entry-point names such as `main000`; there is no common build system or complete dataset bundle. Do not assume a bare compiler command can build the checkout.

## Development and validation

Reproduce a selected paper’s input/output contract on a small graph once dependencies are supplied. No automated test suite exists.

## Related projects and attribution

The original README preserves references to Lappas et al. (2009), Kargar and An (2011), Majumder et al. (2012), Anagnostopoulos et al. (2012), and Kargar et al. (2012).

## License

No root-level license file is included. Check source-specific notices and obtain permission before redistribution or reuse.
