# keyline-bench

Benchmark runs for [keyline](https://github.com/keyline-dev/keyline): every real-model run, kept whole (prompt, every turn and tool call, renders, summary), so a change is judged on runs, not guesses.

- [`reference-ad/`](reference-ad/README.md): Claude Code builds the reference ad through keyline; one folder per run, `results.tsv` across runs.
- [`versus-browser/`](versus-browser/README.md): the same model makes the same images with keyline, HTML + headless Chrome, and Playwright MCP. Its README is the [benchmark page](https://keyline.dev/benchmark/) on keyline.dev.

The harness is keyline's tests (`tests/llm_e2e.rs`, `tests/versus_browser/`). Check this repo out beside keyline as `keyline-bench`, or point `KEYLINE_BENCH` at it, and runs land here. Run them from keyline's root; the commands are in each README.

Licensed like keyline: [FSL-1.1-ALv2](LICENSE).
