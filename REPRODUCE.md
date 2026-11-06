# Reproducing this repository

Input: the Parquet files listed below, revision `fecc2c971945cacd914c63b54ee22db9149e58c9` of the `voilaj/swiss-caselaw` dataset
(`https://huggingface.co/datasets/voilaj/swiss-caselaw/resolve/fecc2c971945cacd914c63b54ee22db9149e58c9/<file>`), plus `graph/statute_references.parquet`
from the same revision, and lexifina/switzerland-law `main` for the overlay's `law_commit`.

```
python tools/build.py gl <cache with data/ and graph/> <empty folder> --today 2026-11-06
```

Needs Python 3 and `duckdb`. Gives 1,421 decision commits and one documentation commit, hash for hash.

## SHA-256 of the input files

```
bfe33b46670a1472e16fdf51a6e2042475d99991f73a2403a372d308cac4a8fb *gl_gerichte.parquet
```
