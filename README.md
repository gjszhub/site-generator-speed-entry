# Site Generator Speed — 22 November 2026

[![make.fun](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/gjszhub/site-generator-speed-entry/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/gjszhub/site-generator-speed-entry/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122)

A faster drop-in for make.fun's own makefun-site 1.0.0: `solve.js` (ES module,
`run(input)` returns makefun-site's answer for every input, byte for byte)
plus `main.ts` (the harness program, answers every case with it).

Practice set: 3/3 cases exact. CPU time ~1.67x faster than the house baseline
makefun-site 1.0.0 on the same machine (median 0.75s vs 1.24s for all 3 cases),
from a run-based Markdown inline renderer, a fused lex-and-render pass,
cached slugs, and a template renderer that appends into one shared parts array.
