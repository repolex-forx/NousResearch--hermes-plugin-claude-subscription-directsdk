# Repolex Knowledge Graph of NousResearch/hermes-plugin-claude-subscription-directsdk

RDF knowledge graph data for [NousResearch/hermes-plugin-claude-subscription-directsdk](https://github.com/NousResearch/hermes-plugin-claude-subscription-directsdk), parsed by [repolex](https://repolex.ai).

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
rlex download NousResearch/hermes-plugin-claude-subscription-directsdk
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ef73726cfaf2fa0ee041e55572f406e2c24fed83
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── ef73726cfaf2fa0ee041e55572f406e2c24fed83.nq.gz
│   └── repolex
│       └── ef73726cfaf2fa0ee041e55572f406e2c24fed83
│           └── chunk-001.nq.gz
├── blob
│   ├── 09d565272067cd89a6e4957b3fd1cc7618d4c771.nq.gz
│   ├── 0a9dab8d2647ab7e945d6f30aadef68040204f84.nq.gz
│   ├── 0d8aad1f0651345decba23cf1b6bc0062e831181.nq.gz
│   ├── 10e16e62c3e00bc8cc47f07c964123ad1b07b005.nq.gz
│   ├── 18836231596fb251577f3c4760250bed4ba45499.nq.gz
│   ├── 1c2e9ebed4f07caa5dd23f421b8323ebce8cd45e.nq.gz
│   ├── 289c9c8150ffb0f1b613c42f3606148afeecd908.nq.gz
│   ├── 3137e5935a5e7d3bb3dfaf6303b56b354a01cf56.nq.gz
│   ├── 4a88fb60f17db28f1307c2f0bf0f76b07f6a1845.nq.gz
│   ├── 4df2667360b75cac437a25d25a20ae99583da2c7.nq.gz
│   ├── 4eb811269203481f0af721a8bb1de2e69437c06c.nq.gz
│   ├── 5592448debb5b8c4427a54eb68c9160edb19b860.nq.gz
│   ├── 5c0fe12146d85090e9ba32dbfb045535cb73e216.nq.gz
│   ├── 5fd853026c63d09d6da0f878623a2f3b77e3d341.nq.gz
│   ├── 6ba469eb046b02f7b80ba493797748771e66b87b.nq.gz
│   ├── 7e28cf135c8e1dd310e7a0fe8587174a5c9e18f1.nq.gz
│   ├── 7ea050bc379db7f26f0e8623c2b4c70e86115304.nq.gz
│   ├── 8eb99711a2efc675815bc13b4c6431099a2cf606.nq.gz
│   ├── b11e797d4d81056fedd9fe1f3544d978a65d9a13.nq.gz
│   ├── bc542b776dd62a8dffc7271f3db3e23c3e380232.nq.gz
│   ├── c160cdafe821839a06c319898592e07cd7156dbc.nq.gz
│   ├── c648ed4d6b15c74153dc88859c3ef77a951ce344.nq.gz
│   ├── d25ef4edd154b2539d9d151b4b6553ad78249066.nq.gz
│   ├── e2381b28ca3c87e1c14af6350414bc0c624e4f69.nq.gz
│   ├── e91647414c987e123051c42c4488b54210336a94.nq.gz
│   └── efd91eda031e81cb418101f7fdca06ff30b586e8.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── ef73726cfaf2fa0ee041e55572f406e2c24fed83.nq.gz
├── filetree
│   └── ef73726cfaf2fa0ee041e55572f406e2c24fed83.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 36 files
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

[NousResearch/hermes-plugin-claude-subscription-directsdk](https://github.com/NousResearch/hermes-plugin-claude-subscription-directsdk)

---
*Parsed on 2026-09-29 by [repolex](https://repolex.ai)*
