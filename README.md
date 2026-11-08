# DnD Bench results

The published results of [DnD-Benchmark/bench](https://github.com/DnD-Benchmark/bench), at [dnd-benchmark.github.io/results](https://dnd-benchmark.github.io/results).

`data/<adventure>.json` holds one summary per game: model, reasoning effort, protocol, seed, task version, the milestones it reached, whether it escaped, its length and cost. They hold no adventure text beyond milestone labels. They're made in a bench checkout with:

```sh
npm run export -- --task scenarios/play/last-gasp.json --out ../results/data/last-gasp.json
```

`index.html` plots milestone share against reasoning effort, one line per model, for a chosen adventure version and protocol.
