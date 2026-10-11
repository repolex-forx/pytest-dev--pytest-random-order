# Repolex Knowledge Graph of pytest-dev/pytest-random-order

RDF knowledge graph data for [pytest-dev/pytest-random-order](https://github.com/pytest-dev/pytest-random-order), parsed by [repolex](https://repolex.ai).

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
rlex download pytest-dev/pytest-random-order
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── cefbff398510b3456e56fd2dda542685efa26db2
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── cefbff398510b3456e56fd2dda542685efa26db2
│           └── chunk-001.nq.gz
├── blob
│   ├── 13373f77aaa4ff4b4b4313e494447ec897bf41bd.nq.gz
│   ├── 1ba385280dc389bb3057cc61b4deeb343273260c.nq.gz
│   ├── 33b5fea8313bfbffabc12658b2ebea509fae3b61.nq.gz
│   ├── 3654f18544c2d0be411713d97e55d3762137b4b8.nq.gz
│   ├── 371f94ab84f594f1b44a033b1b52f8b52af331f1.nq.gz
│   ├── 39c7ad7f76086cadc679ecf3bdd83c980933ab5f.nq.gz
│   ├── 3ca588d6a08878e34e9d1934f36dccbb33383fce.nq.gz
│   ├── 40356044c1905e7a27f85a7d165664a88b00d629.nq.gz
│   ├── 514619acb3bf3da9b2d51e9a02cda4432e2c283f.nq.gz
│   ├── 51d01644a5c5ccaff9e23a6b01b9dc1be82c9696.nq.gz
│   ├── 53c615f0ed0a55c09c03fccdd0c9f43c8d79ee0e.nq.gz
│   ├── 581d91dcd691de8ed2c1e572f3527b7588f93b17.nq.gz
│   ├── 5c3b305fb54fba5e629658a01519599727b8632a.nq.gz
│   ├── 5fee5a927a4833892fd4c82404e77aa8e871f817.nq.gz
│   ├── 6bcda1acb043875bf5bac9078ab07490b142c14a.nq.gz
│   ├── 6ccc855b0a87c000d3b1137bb54a4479e58702ac.nq.gz
│   ├── 78cdfb282077b35c0f88f7dad623718df70d9f37.nq.gz
│   ├── 84f566271f0ed22d88b3ad2edeb8583874d047cc.nq.gz
│   ├── 8818d89822747628b3e23d848d964f51e73af3bb.nq.gz
│   ├── 8bd58def0c691a1d4481361c9475f39ef7b43585.nq.gz
│   ├── 98f92c41637b173a50effeaf89635297a7199e0b.nq.gz
│   ├── afe04199b10dbf93c9e30d33279bf7b50ace5327.nq.gz
│   ├── b5cd150bee5721a928d4af8525b865d9dd84eca8.nq.gz
│   ├── bbadac32161a86c6b9b746a3882c33b39534162c.nq.gz
│   ├── be006de9a1ae3b9628e796c74277cd6d61e0a34a.nq.gz
│   ├── c4720665e53eee77e6ac4dfbc347e40fa79351c3.nq.gz
│   ├── cf332868f167eb6c77929ac02a6c95a56c44ffc3.nq.gz
│   ├── d1fe9b91a75aa7167413bd1386670d3b45591102.nq.gz
│   ├── f20f3d9957c127ea4b5893083f7798d16c3ac26a.nq.gz
│   └── fd51a544e3e8df00f599f1b6b2fa3770c359d2db.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── cefbff398510b3456e56fd2dda542685efa26db2.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 38 files
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

[pytest-dev/pytest-random-order](https://github.com/pytest-dev/pytest-random-order)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
