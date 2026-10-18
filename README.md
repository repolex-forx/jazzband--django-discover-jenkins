# Repolex Knowledge Graph of jazzband/django-discover-jenkins

RDF knowledge graph data for [jazzband/django-discover-jenkins](https://github.com/jazzband/django-discover-jenkins), parsed by [repolex](https://repolex.ai).

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
rlex download jazzband/django-discover-jenkins
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c056f94456f3889a88bbd68cf63838ea31628753
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── c056f94456f3889a88bbd68cf63838ea31628753
│           └── chunk-001.nq.gz
├── blob
│   ├── 05b05d497d7e1ba8b8931d712302e675d2e61026.nq.gz
│   ├── 087a8637212c836bb8da118600926a3d041d1b1c.nq.gz
│   ├── 0fc36a34c27f8863de0560f451ddbfa5fa957f46.nq.gz
│   ├── 16385fa14f1836bf61392e652a3701e619f7fafd.nq.gz
│   ├── 1a9bb6e72cdd91b7734d592a4479f6bc19334fa7.nq.gz
│   ├── 1be56cac26350df0994d2b496feeeb5b92a7684f.nq.gz
│   ├── 1f4132d80346d8a2be098cad7554b4c07bbe2876.nq.gz
│   ├── 2002990eb80a150d4e31c09848b977b5a9696f58.nq.gz
│   ├── 34914f0605f3f3c9f09bf69c0c383b097d76896f.nq.gz
│   ├── 3e292532b53c0e8c7f71ef07f0736aeddf8083bd.nq.gz
│   ├── 4c9e26df48657691f79e1e9d111b2fdef3e8eaf3.nq.gz
│   ├── 550c25a6d29d463e4b670e6f294d8381e51d05b6.nq.gz
│   ├── 58e666c0f7382d44d4fcdc45476084c903a7d9d0.nq.gz
│   ├── 590ede3b58944fd51fe3c24a6fdbb39321642764.nq.gz
│   ├── 5f6299a2d2b103c0f77b55c83039a1b942334a28.nq.gz
│   ├── 61e3f8c5d29187212adfc594fa0a2a441e2435eb.nq.gz
│   ├── 64fc47bf52f080f85769d88f97027bc544de9d32.nq.gz
│   ├── 669ffbd9ef5ee97ec6c5f1707bac2970208331d8.nq.gz
│   ├── 68064711042782bc508668cd8e600104718a9409.nq.gz
│   ├── 6bb006b6036af52c39028f272c5840c78f4d5d76.nq.gz
│   ├── 6d0efade5db8a53e205253c1b6e3805445579c33.nq.gz
│   ├── 7023e1150812f90a0a3d04d5cb061f9c99e4d89a.nq.gz
│   ├── 7ac1f7c094c76f90244aa83379b1760a74962c8c.nq.gz
│   ├── 853eb176baa84d6b187b4c4751079c1813e57a91.nq.gz
│   ├── 864ce0bdb7de0dd9c16bf3a29f817759fb4aee05.nq.gz
│   ├── 907f9ba76e94d39830ca91a7d148e01d151f3741.nq.gz
│   ├── a30814b95a800052aed27377c1e5c06b48e7a97f.nq.gz
│   ├── a993ef560b4eba7b7aa3d259019630987726c30d.nq.gz
│   ├── b40095b93affe92df86bd9049e21f53831129d7e.nq.gz
│   ├── b4082a58fb2283c4cbf31576a1eb1e6b23505d05.nq.gz
│   ├── ba8ad58e763fddab8632124900bd1c48588325b2.nq.gz
│   ├── bb10984719831fc635af02a9580e6e4a8401d6d3.nq.gz
│   ├── d6a0f62c55f14eb6eb18442dd123d459cf872d35.nq.gz
│   ├── db9d8152f6951b6f093173d881ca49f51131b45e.nq.gz
│   ├── df67d44781e431b4ae4f8da953cafa4e55eb2576.nq.gz
│   ├── e0d5efab56fb94577e7804603eb6f21f36977cb2.nq.gz
│   ├── e1de1d5a729502422b1ac32bfd98939e4ce3ce8d.nq.gz
│   ├── e33a311a9e5409649a5e38c4fb85f99d54c8f6ec.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f1e1526e0c09e677c5db82685f0b25ac70b5c3fb.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── c056f94456f3889a88bbd68cf63838ea31628753.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
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

[jazzband/django-discover-jenkins](https://github.com/jazzband/django-discover-jenkins)

---
*Parsed on 2026-10-18 by [repolex](https://repolex.ai)*
