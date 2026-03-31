# Repolex Knowledge Graph of psf/requests

RDF knowledge graph data for [psf/requests](https://github.com/psf/requests), parsed by [repolex](https://repolex.ai).

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
lexq download psf/requests
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│   │   ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│   │   ├── 147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4.nq.gz
│   │   ├── 16c8241a8128920cfc4b64ea41418dbd6f5b36cb.nq.gz
│   │   ├── 18a6b601100db978f3a6e191816456e75bc47e0f.nq.gz
│   │   ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│   │   ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│   │   ├── 282b01a7c9feae30feccbd54e33afcc06197df62.nq.gz
│   │   ├── 2ad18e0e10e7d7ecd5384c378f25ec8821a10a29.nq.gz
│   │   ├── 3235766d67aecc8db3b343f40d190e9d4752c071.nq.gz
│   │   ├── 33735480f77891754304e7f13e3cdf83aaaa76aa.nq.gz
│   │   ├── 3bb13f8fbb9d4ed1a20bd33495cdc087eb062ca0.nq.gz
│   │   ├── 46d646064ca0836a7d7b4d50ea2c762d12ff8ce1.nq.gz
│   │   ├── 5091c15bd71ec934423a71ce1b53668cd15db68f.nq.gz
│   │   ├── 532756803d3b2b7155c31a57f1d5e3cf31224b5d.nq.gz
│   │   ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│   │   ├── 5dcc03945765a7e7b7044b5f41ff5ee8d707c49b.nq.gz
│   │   ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│   │   ├── 6366d3dd190a9e58ca582955cddf7e2ac5f32dcc.nq.gz
│   │   ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│   │   ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│   │   ├── 883caaf145fbe93bd0d208a6b864de9146087312.nq.gz
│   │   ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│   │   ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│   │   ├── a3d7cf3f27e74c28ef30f01e9f2e483570ab042e.nq.gz
│   │   ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│   │   ├── b2289cd2d5d21bd31cf4a818a4e0ff6951b2317a.nq.gz
│   │   ├── b25c87d7cb8d6a18a37fa12442b5f883f9e41741.nq.gz
│   │   ├── b7bd29734022e634634d908e10bbf7a5ac15e76b.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── c9ef5653cc7df3d2eb7d6065ee68294551bdde40.nq.gz
│   │   ├── ca66267d2cf8adc67ed8857f3f57b45ffde21e01.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   │   ├── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
│   │   ├── e4693eba4f429230d482ca50d0a537fc13ea6884.nq.gz
│   │   └── efb4af01271c8c0ddf49457c7096a5bc91edbdad.nq.gz
│   ├── dataflow
│   │   ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│   │   ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│   │   ├── 147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4.nq.gz
│   │   ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│   │   ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│   │   ├── 2ad18e0e10e7d7ecd5384c378f25ec8821a10a29.nq.gz
│   │   ├── 3235766d67aecc8db3b343f40d190e9d4752c071.nq.gz
│   │   ├── 33735480f77891754304e7f13e3cdf83aaaa76aa.nq.gz
│   │   ├── 3bb13f8fbb9d4ed1a20bd33495cdc087eb062ca0.nq.gz
│   │   ├── 46d646064ca0836a7d7b4d50ea2c762d12ff8ce1.nq.gz
│   │   ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│   │   ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│   │   ├── 6366d3dd190a9e58ca582955cddf7e2ac5f32dcc.nq.gz
│   │   ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│   │   ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│   │   ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│   │   ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│   │   ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│   │   ├── b25c87d7cb8d6a18a37fa12442b5f883f9e41741.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   │   └── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
│   ├── lsp
│   │   ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│   │   ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│   │   ├── 147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4.nq.gz
│   │   ├── 16c8241a8128920cfc4b64ea41418dbd6f5b36cb.nq.gz
│   │   ├── 18a6b601100db978f3a6e191816456e75bc47e0f.nq.gz
│   │   ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│   │   ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│   │   ├── 282b01a7c9feae30feccbd54e33afcc06197df62.nq.gz
│   │   ├── 2ad18e0e10e7d7ecd5384c378f25ec8821a10a29.nq.gz
│   │   ├── 3235766d67aecc8db3b343f40d190e9d4752c071.nq.gz
│   │   ├── 33735480f77891754304e7f13e3cdf83aaaa76aa.nq.gz
│   │   ├── 3bb13f8fbb9d4ed1a20bd33495cdc087eb062ca0.nq.gz
│   │   ├── 46d646064ca0836a7d7b4d50ea2c762d12ff8ce1.nq.gz
│   │   ├── 5091c15bd71ec934423a71ce1b53668cd15db68f.nq.gz
│   │   ├── 532756803d3b2b7155c31a57f1d5e3cf31224b5d.nq.gz
│   │   ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│   │   ├── 5dcc03945765a7e7b7044b5f41ff5ee8d707c49b.nq.gz
│   │   ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│   │   ├── 6366d3dd190a9e58ca582955cddf7e2ac5f32dcc.nq.gz
│   │   ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│   │   ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│   │   ├── 883caaf145fbe93bd0d208a6b864de9146087312.nq.gz
│   │   ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│   │   ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│   │   ├── a3d7cf3f27e74c28ef30f01e9f2e483570ab042e.nq.gz
│   │   ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│   │   ├── b2289cd2d5d21bd31cf4a818a4e0ff6951b2317a.nq.gz
│   │   ├── b25c87d7cb8d6a18a37fa12442b5f883f9e41741.nq.gz
│   │   ├── b7bd29734022e634634d908e10bbf7a5ac15e76b.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── c9ef5653cc7df3d2eb7d6065ee68294551bdde40.nq.gz
│   │   ├── ca66267d2cf8adc67ed8857f3f57b45ffde21e01.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   │   ├── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
│   │   ├── e4693eba4f429230d482ca50d0a537fc13ea6884.nq.gz
│   │   └── efb4af01271c8c0ddf49457c7096a5bc91edbdad.nq.gz
│   └── repolex
│       ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│       ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│       ├── 147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4.nq.gz
│       ├── 16c8241a8128920cfc4b64ea41418dbd6f5b36cb.nq.gz
│       ├── 18a6b601100db978f3a6e191816456e75bc47e0f.nq.gz
│       ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│       ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│       ├── 282b01a7c9feae30feccbd54e33afcc06197df62.nq.gz
│       ├── 2ad18e0e10e7d7ecd5384c378f25ec8821a10a29.nq.gz
│       ├── 3235766d67aecc8db3b343f40d190e9d4752c071.nq.gz
│       ├── 33735480f77891754304e7f13e3cdf83aaaa76aa.nq.gz
│       ├── 3bb13f8fbb9d4ed1a20bd33495cdc087eb062ca0.nq.gz
│       ├── 46d646064ca0836a7d7b4d50ea2c762d12ff8ce1.nq.gz
│       ├── 5091c15bd71ec934423a71ce1b53668cd15db68f.nq.gz
│       ├── 532756803d3b2b7155c31a57f1d5e3cf31224b5d.nq.gz
│       ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│       ├── 5dcc03945765a7e7b7044b5f41ff5ee8d707c49b.nq.gz
│       ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│       ├── 6366d3dd190a9e58ca582955cddf7e2ac5f32dcc.nq.gz
│       ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│       ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│       ├── 883caaf145fbe93bd0d208a6b864de9146087312.nq.gz
│       ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│       ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│       ├── a3d7cf3f27e74c28ef30f01e9f2e483570ab042e.nq.gz
│       ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│       ├── b2289cd2d5d21bd31cf4a818a4e0ff6951b2317a.nq.gz
│       ├── b25c87d7cb8d6a18a37fa12442b5f883f9e41741.nq.gz
│       ├── b7bd29734022e634634d908e10bbf7a5ac15e76b.nq.gz
│       ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│       ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│       ├── c9ef5653cc7df3d2eb7d6065ee68294551bdde40.nq.gz
│       ├── ca66267d2cf8adc67ed8857f3f57b45ffde21e01.nq.gz
│       ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│       ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│       ├── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
│       ├── e4693eba4f429230d482ca50d0a537fc13ea6884.nq.gz
│       └── efb4af01271c8c0ddf49457c7096a5bc91edbdad.nq.gz
└── blob
    ├── 0063935ce65a9adb52e1504f0783366f355c0b85.nq.gz
    ├── 0069523a04969dd920ea4b43a497162157729174.nq.gz
    ├── 00b2cd58c891fb121a1f4b02a1557fa906a95e78.nq.gz
    ├── 00f8792b690c763c54286b4802f7a5d006bd6fd0.nq.gz
    ├── 012354574d60cb4304b6077fd4b9a19919d3255d.nq.gz
    ├── 0137c91d961d42ac313114fd5e0750471facfab8.nq.gz
    ├── 014b439182373fc67d6bc72daf5292d87e43b181.nq.gz
    ├── 01a4812f21b7c1149b061f495d26692e49624722.nq.gz
    ├── 01c10638ede3992a41d55c1302c26bf81acecfc1.nq.gz
    ├── 01d853d5cae6fd270027f19407eae3d266fd38d7.nq.gz
    ├── 02593a34ac85fcc8bde63551ff35d05a0458178a.nq.gz
    ├── 027f8e5048c795c2ddcca8da9ca488f6946771c1.nq.gz
    ├── 02e0dd1f1d169bb57d5b3b8996b1868108d93523.nq.gz
    ├── 02e8da75151d64feba210e566246cb4be88d5a62.nq.gz
    ├── 0325a2d8614a1a3c30e3da3716b4bef8e96b3216.nq.gz
    ├── 03a01249ddc11a069f2aa4eeb87227ae3755eb2a.nq.gz
    ├── 03c9dcf3eb8337dd69e68574e58c33012ebb2408.nq.gz
    ├── 0417d6f668c9ae16897ef4d1c80fb5664110a452.nq.gz
    ├── 04512072251c429e63ed110cdbafaf4b3cca3412.nq.gz
    ├── 04ba7e50cda707b30187e288f6dad26e9df80321.nq.gz
    ├── 04f2d7fb4405bb013f12b40692ecb20974fab359.nq.gz
    ├── 0508b1b1abc3f727fe54fdc6653e5310e0105e71.nq.gz
    ├── 051cda1340effaa0706b46dd68ac002ceda3d45c.nq.gz
    ├── 0546a121a5830e5382f7deba37985be1e5172f66.nq.gz
    ├── 055154d01a949305b629905c16454c40f820e024.nq.gz
    ├── 056f6fb3caf0dfb21e2df9cc7adb6216c6e4b75b.nq.gz
    ├── 05d2b3f57beadb7dd36718487281e746d96de014.nq.gz
    ├── 060d9262a5e763c78a707222600a02f4c3b5fd66.nq.gz
    ├── 063d5f96a8aff4906b0cb9864d48718b7bdc58b6.nq.gz
    ├── 064345b0867d4d23ef17a4d7d11663dcf3cf4adf.nq.gz
    ├── 0658e7ec5099072633767b69e646b6827094ab12.nq.gz
    ├── 068e9cf801a5b5ddbb57bd1bb9ea2a3535b90928.nq.gz
    ├── 06e06b2a750f4d30024e92cb48f25fc09b6bd41d.nq.gz
    ├── 06e17d4b94d80f98e53eca961c0375268dcc41de.nq.gz
    ├── 0716c65c9a295eccb86c59b3b37cc5ae65aad3fc.nq.gz
    ├── 0737bd319a2a53dea3c99a663df701221ed68efe.nq.gz
    ├── 075d042ac85d7c8dc7f0e9839026955483bd035b.nq.gz
    ├── 07698f6f6ee89a319bf32d0be6089238002c665e.nq.gz
    ├── 07e64750703903bd3971aa7536f6605ae65d6759.nq.gz
    ├── 0820d59c379e055c0a4a1c52adb0aaa8128cbb15.nq.gz
    ├── 08a2acf6dcaaf4fbdc0422fe7cca72a30a1e2a0a.nq.gz
    ├── 08ba2bc6f12d8e9a61e175a366fe0261de84a52f.nq.gz
    ├── 08cb1b8d1f35e05eba6f48a7ff02e87f79873409.nq.gz
    ├── 08edab4e17fb773bc60bf3bba98b0e095cc67a4e.nq.gz
    ├── 093f45edc7f02afb28589237bb3a615eb6b4a227.nq.gz
    ├── 09446b34f8a1ed86b925dbebbb0b6cb9d09dbbc2.nq.gz
    ├── 098193f88d9bacd97a91aecaf874ac584977ac94.nq.gz
    ├── 0998d9a4686edf83c71f61b5e2049c1733e43a19.nq.gz
    ├── 09b549014ccde6ef78029c2cb08b317a1121add9.nq.gz
    ├── 09c0c08c84504c235fcfc91ff6e1de31495e96b7.nq.gz
    ├── 09fcb6de1cfd626f06c586f4d1066c55435539b1.nq.gz
    ├── 0a0515cf87a37464c11056127db6cc617b2f31ec.nq.gz
    ├── 0a764a4de3a890dbe2a3336c648f7f6d1892c132.nq.gz
    ├── 0a87b52cdaad377122d606202b581546372652ad.nq.gz
    ├── 0ace12b6964c0cff7772ce959dc691b3831f56c7.nq.gz
    ├── 0adb51de5a210aa36849cd149ed0f4ae424fce42.nq.gz
    ├── 0adca690cde8de6321cf52b2e0c8957b3d917727.nq.gz
    ├── 0adfa0f5d174c49b7c09ee20388d407f010cbf58.nq.gz
    ├── 0ae2182eb19880acda28f4ee8b0ab4cf4b671025.nq.gz
    ├── 0b24e0ff8c1c1f128f2a52ee444d5b6576563d77.nq.gz
    ├── 0b37e57f717480b0da59932d58d99004b27e78d6.nq.gz
    └── 0b5c75c13c8d2f0eaaea3889d72eadd7d493e826.nq.gz

7 directories, 200 files
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

[psf/requests](https://github.com/psf/requests)

---
*Parsed on 2026-03-31 by [repolex](https://repolex.ai)*
