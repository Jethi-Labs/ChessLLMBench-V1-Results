# ChessLLMBench V1.0.0 Official Tournament Results

This is the completed official v1.0.0 team tournament dataset produced on 2026-09-25.

| Field | Value |
| --- | --- |
| Tournament ID | `30dc37793deb105097824217` |
| Teams | 11 |
| Individual bot sources | 110 (10 per team) |
| Completed games | 2,750 |
| Time control | 10+0.1 (10,000 ms + 100 ms increment) |
| Opening pool | v1, 50 positions |
| Team schedule | Interleaved Olympiad-style, schedule v2 |
| Runtime | Linux x86-64, strict sandbox, one worker |

The run archive contains the canonical manifest, deterministic game schedule, pair opening selections, 2,750 individual JSON game records, 2,750 PGNs, team and player leaderboards, pairwise score matrices, and the exact compiled bot executables used for hash verification. Exact bot source files are in the [`ChessLLMBench-V1-Bots`](https://github.com/Jethi-Labs/ChessLLMBench-V1-Bots) repository. Binary files are supplied under `binaries/` and are tied to their recorded SHA-256 values; they are Linux x86-64 artifacts, not portable builds.

To verify after checking this repository out at `results/30dc37793deb105097824217` inside the framework checkout, run from the framework repository root:

```sh
./build/chessbench verify results/30dc37793deb105097824217
```

The manifests use repository-relative source and binary paths so the archived run can be checked out reproducibly. The empty per-game stdout/stderr capture files (11,000 zero-byte files) are omitted; their omission does not affect game records or verification. Raw model API request/response traces are not part of this public dataset.

## Licensing

No separate license is granted to generated bot submissions or this tournament dataset. The framework code is licensed independently under MIT. Contact Jethi Labs about reuse rights.
