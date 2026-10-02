# Repolex Knowledge Graph of block/braindump

RDF knowledge graph data for [block/braindump](https://github.com/block/braindump), parsed by [repolex](https://repolex.ai).

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
rlex download block/braindump
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d267ace6b39a5c2a12657915cb4b4a9379f76386
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── d267ace6b39a5c2a12657915cb4b4a9379f76386.nq.gz
│   └── repolex
│       └── d267ace6b39a5c2a12657915cb4b4a9379f76386
│           └── chunk-001.nq.gz
├── blob
│   ├── 0367d2331a2cbfb3dadb43da08affe106a235c28.nq.gz
│   ├── 0ba9db25329d0b336e39ca8cde8470c5b7bc45eb.nq.gz
│   ├── 0e6569b7ea6147c031dcd1eac0690ee889f9ecd6.nq.gz
│   ├── 0fc1b616d7c4a0c81eafeee5c115f447470eea28.nq.gz
│   ├── 17de3a67a94b28f3eb8c49e12648391a5488a2d4.nq.gz
│   ├── 1ffc371d0c83fa0ce4298ab768c87ecf43c08f76.nq.gz
│   ├── 21ecf13a6fc9700d6494b5a930d156bd547e15c7.nq.gz
│   ├── 2302711cc753dbcb585b058a134f0a880906b8c1.nq.gz
│   ├── 25f0bc5ed80683a81f46e6bfd1cf8ea0b56c6807.nq.gz
│   ├── 31559b7d115e3c105b328cce9b9dcd9774025061.nq.gz
│   ├── 383f4511d444516caed0fd113ee8a2b640cd2290.nq.gz
│   ├── 4011a855305149d4a4d55cd70eafb0e60cb323b8.nq.gz
│   ├── 445a45150c4bb374e11ab70a00816e8f1bc14af7.nq.gz
│   ├── 59e5c7a454e7014d90f3913e8f412c0823fc383a.nq.gz
│   ├── 60265c9b5a3072fa1f78a8cd68e9a191f81eb37f.nq.gz
│   ├── 6bccf43368fd7c96d9c659562a5142b8b8cb98a1.nq.gz
│   ├── 6d6b543987bf1c4f35446ad1a5826b755281c7f9.nq.gz
│   ├── 804ec119ac37815ed19996305e60c030b055d894.nq.gz
│   ├── 816066f4755caecbea428ebfe33fecd477e0bb7e.nq.gz
│   ├── 862ee3c28647e7a58801a75236855c269c1448ae.nq.gz
│   ├── 91791d1169cb728dc37f091c3573a99c718168d8.nq.gz
│   ├── 9582fc588754f78d9875691a3bd5e674295436b3.nq.gz
│   ├── a2a2c7f3f495b7e5f4d259ac154e57c64cbad596.nq.gz
│   ├── b04085f1bdac7436fbb4ff694aac62eaf960bdbc.nq.gz
│   ├── b0691ad23789e2b713a0b86552ae85ec9a21facc.nq.gz
│   ├── b17156ee547b7ee605699aadf06647389a2186d3.nq.gz
│   ├── b1b02b9188f1cf3fdf16bbbf3fa9223e7c1c3f1d.nq.gz
│   ├── b2c31046c3fa6eda1ab9c05f6ee3a579c9abe782.nq.gz
│   ├── b2e9b64c7d03a3b0c6c5f72dd349119a7bf9c5f6.nq.gz
│   ├── b4e2d02cbcfbef1b5ff08eed03be2a1bb7cd4650.nq.gz
│   ├── b843e27a0f23e6136ae47b2d63cdddb580be0382.nq.gz
│   ├── c0e47fb3182bd05d1e3aa8b134a1351de8076636.nq.gz
│   ├── d03447fc35986694d3d09468b7511d145a135178.nq.gz
│   ├── e889550ba4cbc92a720527042e5f6e7a303bfcbc.nq.gz
│   ├── eabd38531bb82650598a347c668f4c076ec20787.nq.gz
│   ├── f0e42af466b703cc22812c5a3ed7caeaaef22b47.nq.gz
│   ├── fa98825320cd58438453f876ed5f6ae8b02b4f06.nq.gz
│   ├── fba163d5741edfbe9604f1d94795455e64c25718.nq.gz
│   ├── fe0867819936afc4af0bf1512d453bc7465e7db2.nq.gz
│   └── fe28214d3352b0ed40820a4999317694c8b1ef57.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── d267ace6b39a5c2a12657915cb4b4a9379f76386.nq.gz
├── filetree
│   └── d267ace6b39a5c2a12657915cb4b4a9379f76386.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 50 files
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

[block/braindump](https://github.com/block/braindump)

---
*Parsed on 2026-10-02 by [repolex](https://repolex.ai)*
