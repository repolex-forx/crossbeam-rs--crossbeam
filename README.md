# Repolex Knowledge Graph of crossbeam-rs/crossbeam

RDF knowledge graph data for [crossbeam-rs/crossbeam](https://github.com/crossbeam-rs/crossbeam), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download crossbeam-rs/crossbeam
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 7e8f008a69f152a66984e3867f36d79e18a3d242
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 7e8f008a69f152a66984e3867f36d79e18a3d242.nq.gz
│   └── repolex
│       └── 7e8f008a69f152a66984e3867f36d79e18a3d242
│           └── chunk-001.nq.gz
├── blob
│   ├── 128aad30ac7556dfcb05379a77ccea8dd620c06e.nq.gz
│   ├── 143b1ca0147427236f1dd485fa0972d492eada75.nq.gz
│   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│   ├── 236e106d63165fa24ee9eccaa2c80cce67916d16.nq.gz
│   ├── 25597d5838fa4cd7ff5c3c2bb1d1b4c3731eda7f.nq.gz
│   ├── 97e2c9f321ce824052d3d58167543b8306b8a730.nq.gz
│   ├── 9b9ac505885cf5fd0ebc611c9b2de3c1eca3ba4e.nq.gz
│   ├── a121930405f021c5600122342865a4e38f8250f4.nq.gz
│   ├── bf13c7e1657a595ac0410d6d35575bc2770ab698.nq.gz
│   └── e8f5b4d39312e1f2f2de8905dc5589fa0309fd31.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 7e8f008a69f152a66984e3867f36d79e18a3d242.nq.gz
├── filetree
│   └── 7e8f008a69f152a66984e3867f36d79e18a3d242.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 20 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |

## Source repository

[crossbeam-rs/crossbeam](https://github.com/crossbeam-rs/crossbeam)

---
*Parsed on 2026-04-23 by [repolex](https://repolex.ai)*
