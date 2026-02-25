# Rtemporaria
Functional annotation R package (v1) for the common frog (Rana temporaria)
# org.Rtemporaria.eg.db

An organism annotation package for the common frog *Rana temporaria*, providing gene-level mappings in an `AnnotationDbi` SQLite database (similar to Bioconductor `org.*.eg.db` packages).

This package is intended to support downstream analyses such as:
- gene ID conversion (e.g., transcript/protein IDs → gene IDs, SYMBOL-like IDs, etc.)
- GO term annotation and enrichment analysis workflows (via `AnnotationDbi`, `clusterProfiler`, etc.)

> Package archive name on GitHub: `org.Rtemporaria.eg.db_1.0.tar.gz`

---

## What this package is

`org.Rtemporaria.eg.db` is an R annotation package built on top of **AnnotationDbi**.  
It stores *Rana temporaria* gene annotations in a local **SQLite** database and exposes them through standard Bioconductor-style APIs.

Typical operations include:
- listing supported key types and columns
- retrieving annotations using `select()`, `mapIds()`, etc.
- converting identifiers for enrichment pipelines

---

## Installation

Download `org.Rtemporaria.eg.db_1.0.tar.gz` and install locally:

```r
install.packages("org.Rtemporaria.eg.db_1.0.tar.gz", repos = NULL, type = "source")
