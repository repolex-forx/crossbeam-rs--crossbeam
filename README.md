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
│   │   ├── 76f6b7cac1e5e827279c05acdb8a2739f164a54f
│   │   │   └── chunk-001.nq.gz
│   │   ├── 7e8f008a69f152a66984e3867f36d79e18a3d242
│   │   │   └── chunk-001.nq.gz
│   │   ├── 8f353c52e918029466e42cd0eefc34849c15c532
│   │   │   └── chunk-001.nq.gz
│   │   └── f36df0fc8d4814f4b449f55247bc6246fa1a33b5
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 7e8f008a69f152a66984e3867f36d79e18a3d242.nq.gz
│   │   └── 8f353c52e918029466e42cd0eefc34849c15c532.nq.gz
│   └── repolex
│       ├── 7e8f008a69f152a66984e3867f36d79e18a3d242
│       │   └── chunk-001.nq.gz
│       └── 8f353c52e918029466e42cd0eefc34849c15c532
│           └── chunk-001.nq.gz
├── blob
│   ├── 050c3531e7bea962c128ab1966a69bac76b04b42.nq.gz
│   ├── 0726401732428ae70ddbbf85630adf9e34d7b9de.nq.gz
│   ├── 10307e2ed6c5b648b320eb526148c076e4bd4be1.nq.gz
│   ├── 128aad30ac7556dfcb05379a77ccea8dd620c06e.nq.gz
│   ├── 143b1ca0147427236f1dd485fa0972d492eada75.nq.gz
│   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│   ├── 1a0f89e2063070f6af99cdfb37cc0e830f84cdae.nq.gz
│   ├── 236e106d63165fa24ee9eccaa2c80cce67916d16.nq.gz
│   ├── 25597d5838fa4cd7ff5c3c2bb1d1b4c3731eda7f.nq.gz
│   ├── 2f473c448a964362be5b04ac94f63d4fe63ac5b3.nq.gz
│   ├── 3063f9829c90de6ebe00cea313c93febcff91a28.nq.gz
│   ├── 3ac7ae6da19a95b0f5b6dca3fb24401b05b6eb7a.nq.gz
│   ├── 3b890cd011f0ac667a9c6790264677359c486f03.nq.gz
│   ├── 42d12733d36cf1ee7894b00dbf20bdbc494296f8.nq.gz
│   ├── 42f3ab3bab965316dabc5ddd746ca4137e577a17.nq.gz
│   ├── 478f262dcc963df1ccbc9063f4f295cca3a9c695.nq.gz
│   ├── 485946a9fea8e954e97d2930af858fd5907935e0.nq.gz
│   ├── 5023c1105ccb911f01004333ced055f3d9a1641a.nq.gz
│   ├── 51076bbaa15724bda42da3c702e6193f0a624556.nq.gz
│   ├── 55554bcb2ffc147ec899a5b8c22e498b87014ac6.nq.gz
│   ├── 5d0752e42cbcbee597a78132b48bdb3a8b089f23.nq.gz
│   ├── 5eb2167ea4f775d7d052efb42bf407bba05f4517.nq.gz
│   ├── 5f6dbcc376597e2271b8133ded68190a4033fced.nq.gz
│   ├── 646fce953770c2340da85adc3c1bd797bd2ac906.nq.gz
│   ├── 66230f49e8d72baf0547cd5c21d3dfe871e042a7.nq.gz
│   ├── 6737d9d0c808c2eb0c7f632711d5985db02394c6.nq.gz
│   ├── 676328bfaae4f5af9a884e69be21b8113ab187d2.nq.gz
│   ├── 6a05fd0d98a48a672db2568406a5269b60e3b3a1.nq.gz
│   ├── 6aa106405a4b4a00d779beab77c90c9473a6d203.nq.gz
│   ├── 6f5f8fc1991b368d462d3c0de30df3a22eda6702.nq.gz
│   ├── 6f6e0a760f2a894e54ad59674b863580d61b79ea.nq.gz
│   ├── 7501040d2ef8aa5069c2c8e7f6ffa13b47cc31dd.nq.gz
│   ├── 7e692baafb4c929b0b5f0764d9f7be7d16d24b32.nq.gz
│   ├── 7f3eeaf0a97c915d21b2d078f45cb740f4873ba0.nq.gz
│   ├── 880246dbe0fdf80e74d15141072d498547f82ecb.nq.gz
│   ├── 8ba99d5be1da554b6b93fa7cf8ebf9f7cf245cc7.nq.gz
│   ├── 8f5d9af1579f0eb66fb9bef26b837fc8464ba95c.nq.gz
│   ├── 90639b7a6fb3cc80dec241abbda94cdd18863473.nq.gz
│   ├── 97e2c9f321ce824052d3d58167543b8306b8a730.nq.gz
│   ├── 9b9ac505885cf5fd0ebc611c9b2de3c1eca3ba4e.nq.gz
│   ├── a121930405f021c5600122342865a4e38f8250f4.nq.gz
│   ├── a538f81346cf261179d6ed8f8408abc0c5863aa4.nq.gz
│   ├── ac67fbd75b351958f59ebcb1836909910e231867.nq.gz
│   ├── b288d9b2c01332ef9c3286e1d450755282b420c8.nq.gz
│   ├── b544faf431f616fbb9b6684c3f69ca4d4f27b14d.nq.gz
│   ├── bf13c7e1657a595ac0410d6d35575bc2770ab698.nq.gz
│   ├── c204fc869694a94755de1b582f08caeda1d06f46.nq.gz
│   ├── c9e6185c8e72cb7953bc98a364f1cd9a2dfb6e6d.nq.gz
│   ├── ca98cd96efdc228b0c0d0e264bfc0ce9ddadfdd7.nq.gz
│   ├── d675a1ad75029e342ef80ebcb78c75ca480d26c6.nq.gz
│   ├── e67680be87b68d9cd3db982e5acd78fed34535bf.nq.gz
│   ├── e686bdba0d5a818f0c2e7bc57031c866969bff31.nq.gz
│   ├── e69282e381bc07152cc7598f21f3162e4bbb1f22.nq.gz
│   ├── e8f5b4d39312e1f2f2de8905dc5589fa0309fd31.nq.gz
│   ├── e94231e9174ca5e26cfd65c838873ffa033e93ae.nq.gz
│   ├── f524e7e170bffc2f962ab802c5e432096d46da81.nq.gz
│   ├── f8eb25960029b2ae83b7b4a824d1bb736b643093.nq.gz
│   ├── f932d4f36fd3aca9e4ffa7b874d4cd9e9b735802.nq.gz
│   ├── fa6d6c852184858c706853be4b9ef5757d7312fa.nq.gz
│   ├── faf10f8999497614a4b2ed10fc0902869702f7a0.nq.gz
│   ├── fb7ce38204bbb65d6d1e37a8562bff4f38b6fd80.nq.gz
│   └── fdf53b440ef6fe5b3c0d69c920c2a20e5647727b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 7e8f008a69f152a66984e3867f36d79e18a3d242.nq.gz
│   └── 8f353c52e918029466e42cd0eefc34849c15c532.nq.gz
├── filetree
│   ├── 09a9346b68c68c5c3002b9b7b05853342f6414cd.nq.gz
│   ├── 76f6b7cac1e5e827279c05acdb8a2739f164a54f.nq.gz
│   ├── 7e8f008a69f152a66984e3867f36d79e18a3d242.nq.gz
│   ├── 8f353c52e918029466e42cd0eefc34849c15c532.nq.gz
│   ├── af60549fcb61424dafbf85bbbbb9ced681f9ebda.nq.gz
│   └── f36df0fc8d4814f4b449f55247bc6246fa1a33b5.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

19 directories, 83 files
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
*Parsed on 2026-05-10 by [repolex](https://repolex.ai)*
