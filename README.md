# Unique Name Viewer

Static, client-side viewer for extracted-name diversity results from LM outputs: the
unique names counted per file (under the production counting rule, with the rule before
2026-09-29 beside it for k = 1 and 3), the items the extractor marked incorrect, and the
list-length experiment (k = 5 ... 1000 items per answer). **Live:** https://seuneisape.github.io/name-viewer/

Rebuilt with `utils/build_name_viewer.py` in the source repo: a small `index.json.gz`
loaded up front plus lazy-loaded per-group shards under `details/`.

**NVBench generations viewer:** [nvbench.html](nvbench.html) — the N generations per
prompt across every model & run, colored by NoveltyBench partition cluster (built with
`utils/build_nvbench_viewer.py`).
