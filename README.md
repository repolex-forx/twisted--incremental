# Repolex Knowledge Graph of twisted/incremental

RDF knowledge graph data for [twisted/incremental](https://github.com/twisted/incremental), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download twisted/incremental
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 830ebeddf654cb39fb3a19493888588a8ba8e907
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 830ebeddf654cb39fb3a19493888588a8ba8e907
│           └── chunk-001.nq.gz
├── blob
│   ├── 00bb4d2155a098bd951cc47dd1fdf5704075d397.nq.gz
│   ├── 00e382a10e547f165c294420b2f42563a781a27d.nq.gz
│   ├── 073c510771499daea432b8e2cf6dad9beaff0e2b.nq.gz
│   ├── 089e0cd4170e57de1b5fef18180ea64a5222f8c9.nq.gz
│   ├── 0ae478d05c2e708788de0dcfc9ac06f681d5ac81.nq.gz
│   ├── 26d23badb640c01b8f8ddfae656ddff9b9723223.nq.gz
│   ├── 279c77b77781b70d6b7bdb082ab37c27856e3a6e.nq.gz
│   ├── 2a3189e253c66f1d633411be62cc308299fa8dd3.nq.gz
│   ├── 2d606e4c989b2ca7d9e481c43ee70461a68d9f06.nq.gz
│   ├── 314892989b13406cff962111d4a4f67049e47cc3.nq.gz
│   ├── 374fa3414d895c8b22fdbb84df0b253eeabb97da.nq.gz
│   ├── 39416a5be46accc242d2cafee5f1ef1e10739554.nq.gz
│   ├── 39a8911baca15b933d79d09676d4cad91b5cce3f.nq.gz
│   ├── 3f63da0101492901a300c0e4bea9f1f69267f56d.nq.gz
│   ├── 3f809ff0e3d614e005d569393d3fc1ab3cbb56f6.nq.gz
│   ├── 42793030d15e52e60a44ee58ffd8383bced5ae44.nq.gz
│   ├── 53b56f0619efae9b03601cc055347b156e653dd3.nq.gz
│   ├── 69b8e06771d6b18b9e17cc68ef557d78eb7e233b.nq.gz
│   ├── 6f1e6b0bcb70f625616d094cb1b17ab336516abb.nq.gz
│   ├── 7d61bbfa0982b97c623379a8aa689014366361d4.nq.gz
│   ├── 82ca44a313f49baf79b9d6934a7465898421c229.nq.gz
│   ├── 8e00e35260b2cfd5f8c2ed64edfbbf3aa42bd4d1.nq.gz
│   ├── 90e63652a6d0fca9e67ae9aa7567768403b6962f.nq.gz
│   ├── 92d9e042dc8c7e7292f95a6d12a9ceed2f61bc74.nq.gz
│   ├── 956be5fe33e2c2295f65dc02e9bcd65aa655f5a3.nq.gz
│   ├── af3ee5763862e3daa29c9085c29d1c64cc60edd5.nq.gz
│   ├── afec27ddf0c3a4af3797c449e544d8ec758a65f2.nq.gz
│   ├── b0af258ec3b733d98531f60c3323c6e98f9cd243.nq.gz
│   ├── b7ad7c9f69a6efcd95bdd28c17593eb867408e09.nq.gz
│   ├── baa891687a9b5fb74df0ed43d65671ab5f3de50e.nq.gz
│   ├── bc9d47f3322bf13a1442e2b6c1e5e5edea3f886a.nq.gz
│   ├── beca60e18b8f34968ca669f9c19803bde3e36af3.nq.gz
│   ├── c678d10da05a437e62ad81ece63d5f0c0ca5900f.nq.gz
│   ├── ce02d5647ddd9b4c65fce0631a9b08706782796a.nq.gz
│   ├── d905bf2339c9d93e5b4c528255eeedc72339776a.nq.gz
│   ├── dc186c1036cf916a18fa77c0fcad9fa87c04e458.nq.gz
│   ├── e39c43fffa7db69fc58f01db416560e69dd70364.nq.gz
│   ├── e4ce3e396481e446253cd306aa62ac14439bcb96.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f2feb544faf271b946725dd33b5dc03058548293.nq.gz
│   ├── f935021a8f8a7bd22f9d6703cafa5134bb6a57f8.nq.gz
│   ├── fa017450db37f12561307da4967728569fe99715.nq.gz
│   └── fef740f835863f188bd7cd59bdeebe57d0e4d245.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 830ebeddf654cb39fb3a19493888588a8ba8e907.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 51 files
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
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[twisted/incremental](https://github.com/twisted/incremental)

---
*Parsed on 2026-10-12 by [repolex](https://repolex.ai)*
