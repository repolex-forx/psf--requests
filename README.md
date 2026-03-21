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
│   │   ├── b7bd29734022e634634d908e10bbf7a5ac15e76b.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── ca66267d2cf8adc67ed8857f3f57b45ffde21e01.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   │   └── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
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
│   │   ├── b7bd29734022e634634d908e10bbf7a5ac15e76b.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── ca66267d2cf8adc67ed8857f3f57b45ffde21e01.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   │   └── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
│   └── repolex
│       ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│       ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│       ├── 147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4.nq.gz
│       ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│       ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│       ├── 2ad18e0e10e7d7ecd5384c378f25ec8821a10a29.nq.gz
│       ├── 3235766d67aecc8db3b343f40d190e9d4752c071.nq.gz
│       ├── 33735480f77891754304e7f13e3cdf83aaaa76aa.nq.gz
│       ├── 3bb13f8fbb9d4ed1a20bd33495cdc087eb062ca0.nq.gz
│       ├── 46d646064ca0836a7d7b4d50ea2c762d12ff8ce1.nq.gz
│       ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│       ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│       ├── 6366d3dd190a9e58ca582955cddf7e2ac5f32dcc.nq.gz
│       ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│       ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│       ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│       ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│       ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│       ├── b25c87d7cb8d6a18a37fa12442b5f883f9e41741.nq.gz
│       ├── b7bd29734022e634634d908e10bbf7a5ac15e76b.nq.gz
│       ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│       ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│       ├── ca66267d2cf8adc67ed8857f3f57b45ffde21e01.nq.gz
│       ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│       ├── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│       └── dd777b3d7e8975ec6927dc9cc15b881778d39bc8.nq.gz
└── blob
    ├── 0063935ce65a9adb52e1504f0783366f355c0b85.nq.gz
    ├── 00b2cd58c891fb121a1f4b02a1557fa906a95e78.nq.gz
    ├── 012354574d60cb4304b6077fd4b9a19919d3255d.nq.gz
    ├── 0137c91d961d42ac313114fd5e0750471facfab8.nq.gz
    ├── 01a4812f21b7c1149b061f495d26692e49624722.nq.gz
    ├── 01c10638ede3992a41d55c1302c26bf81acecfc1.nq.gz
    ├── 01d853d5cae6fd270027f19407eae3d266fd38d7.nq.gz
    ├── 027f8e5048c795c2ddcca8da9ca488f6946771c1.nq.gz
    ├── 02e0dd1f1d169bb57d5b3b8996b1868108d93523.nq.gz
    ├── 0325a2d8614a1a3c30e3da3716b4bef8e96b3216.nq.gz
    ├── 03a01249ddc11a069f2aa4eeb87227ae3755eb2a.nq.gz
    ├── 03c9dcf3eb8337dd69e68574e58c33012ebb2408.nq.gz
    ├── 0417d6f668c9ae16897ef4d1c80fb5664110a452.nq.gz
    ├── 04ba7e50cda707b30187e288f6dad26e9df80321.nq.gz
    ├── 04f2d7fb4405bb013f12b40692ecb20974fab359.nq.gz
    ├── 0508b1b1abc3f727fe54fdc6653e5310e0105e71.nq.gz
    ├── 051cda1340effaa0706b46dd68ac002ceda3d45c.nq.gz
    ├── 0546a121a5830e5382f7deba37985be1e5172f66.nq.gz
    ├── 055154d01a949305b629905c16454c40f820e024.nq.gz
    ├── 060d9262a5e763c78a707222600a02f4c3b5fd66.nq.gz
    ├── 063d5f96a8aff4906b0cb9864d48718b7bdc58b6.nq.gz
    ├── 064345b0867d4d23ef17a4d7d11663dcf3cf4adf.nq.gz
    ├── 06e17d4b94d80f98e53eca961c0375268dcc41de.nq.gz
    ├── 0716c65c9a295eccb86c59b3b37cc5ae65aad3fc.nq.gz
    ├── 0737bd319a2a53dea3c99a663df701221ed68efe.nq.gz
    ├── 07698f6f6ee89a319bf32d0be6089238002c665e.nq.gz
    ├── 07e64750703903bd3971aa7536f6605ae65d6759.nq.gz
    ├── 0820d59c379e055c0a4a1c52adb0aaa8128cbb15.nq.gz
    ├── 08a2acf6dcaaf4fbdc0422fe7cca72a30a1e2a0a.nq.gz
    ├── 08ba2bc6f12d8e9a61e175a366fe0261de84a52f.nq.gz
    ├── 08cb1b8d1f35e05eba6f48a7ff02e87f79873409.nq.gz
    ├── 08edab4e17fb773bc60bf3bba98b0e095cc67a4e.nq.gz
    ├── 09446b34f8a1ed86b925dbebbb0b6cb9d09dbbc2.nq.gz
    ├── 098193f88d9bacd97a91aecaf874ac584977ac94.nq.gz
    ├── 09b549014ccde6ef78029c2cb08b317a1121add9.nq.gz
    ├── 09fcb6de1cfd626f06c586f4d1066c55435539b1.nq.gz
    ├── 0a0515cf87a37464c11056127db6cc617b2f31ec.nq.gz
    ├── 0a764a4de3a890dbe2a3336c648f7f6d1892c132.nq.gz
    ├── 0a87b52cdaad377122d606202b581546372652ad.nq.gz
    ├── 0ace12b6964c0cff7772ce959dc691b3831f56c7.nq.gz
    ├── 0adca690cde8de6321cf52b2e0c8957b3d917727.nq.gz
    ├── 0adfa0f5d174c49b7c09ee20388d407f010cbf58.nq.gz
    ├── 0ae2182eb19880acda28f4ee8b0ab4cf4b671025.nq.gz
    ├── 0b5c75c13c8d2f0eaaea3889d72eadd7d493e826.nq.gz
    ├── 0b725cae94caf79feaedca0d5ea16578888b27d2.nq.gz
    ├── 0c82c7b46f7664c42031fb85f7355c995aad76d5.nq.gz
    ├── 0cda6591ae53896dfd866da5ab00030513064456.nq.gz
    ├── 0d0d216d5505a3ef879c63a0a54fb2c9044d1900.nq.gz
    ├── 0d61a572df619d5538c6db07af3b9db60d65f587.nq.gz
    ├── 0d6f69d6fe78501131f4a7e5bdbed4ed66911a27.nq.gz
    ├── 0d93893b9df9f6458431d72edf6b515e728df563.nq.gz
    ├── 0e0405ce3afd69dd9653276e6edf91e09aba4ea1.nq.gz
    ├── 0e0dd67f649def8d0eb44a653148883867ac4464.nq.gz
    ├── 0e274101cd5933b4e5408efbf1e6ab8709b77932.nq.gz
    ├── 0e2c719e08549d4bd8123abc65686e57780ccc5f.nq.gz
    ├── 0e3091d0e40052019bc4faeff6c2bc097e9ad148.nq.gz
    ├── 0e7836db1c23062596e1690dcab11dc47f3d2789.nq.gz
    ├── 0e80eaa24a24a9f60546b1962af368e0783ef5af.nq.gz
    ├── 0e8933cf1edb7bd1fc34b79970aa346891cdd6b7.nq.gz
    ├── 0eb7b2f31de03f0c61e5bc633287b7d10b0121b7.nq.gz
    ├── 0eec48db850d6be1d52b837928266742b92f2dc7.nq.gz
    ├── 0f6d9ca93717e81aced697a57d10da8ac547ec97.nq.gz
    ├── 0fb8d7052adcb894d940db7874e633ed934dfcdb.nq.gz
    ├── 0fbf488dfeeb92abdf5b2923f82566fd8ee0216a.nq.gz
    ├── 0ff9c2987455f6b274ba66550977fc20030b1485.nq.gz
    ├── 101d1ce6007eb1e6d2e357f76be1fa91231508a2.nq.gz
    ├── 1023dcba38848fab2185abf32b7165a4f20a9e6c.nq.gz
    ├── 112bbd1eafb35c5c02beecc200f57b59c1792300.nq.gz
    ├── 1140a523f59bca36cffedab8af8d18eb34e03743.nq.gz
    ├── 117269aca4d6420e55de148d31862a2ba1648868.nq.gz
    ├── 11d0b5c34d6c9f6471cd3cafc83dd23ac3ffac9b.nq.gz
    ├── 120968ff5119363bb5c569c1d9398f2b52cabf31.nq.gz
    ├── 1238f510fc6afe2739f3f7a44359cfe471c154a3.nq.gz
    ├── 124458818d77f3e410d89f0aa9caf96f3d8c46f7.nq.gz
    ├── 12b24c9e6751ba567ccb5fb8ae1482e27f7007d2.nq.gz
    ├── 12db07cd00038169e9a0844a1e6d663d8fa43e1d.nq.gz
    ├── 12e1fd77ff1ef7b4ac198c7002f7d9a500cc5a99.nq.gz
    ├── 1305d3f8f01aafea6401621185c0c9cafcb324d4.nq.gz
    ├── 131c0f61c7e06072e040d52b5c0a9695f851d864.nq.gz
    ├── 139334ab6660f597c44c2b4d741e4b72ed72d46b.nq.gz
    ├── 13d0eb5c25ebda4328398ffa971efa311be4d2bb.nq.gz
    ├── 13d44df96deb0cbd378b5db8b402454213bb11fc.nq.gz
    ├── 145838f2009ea1228c8d71dcac37636fbd173cb1.nq.gz
    ├── 1463fa1d85c86785b16efc6663602ff736105cae.nq.gz
    ├── 1473d1258b24a3bd0d024026af3f81938b6a6a86.nq.gz
    ├── 149016d3b1d3d783f166384e51cb8cb96f66d5c7.nq.gz
    ├── 1507609a6b58675b8cf9c10e5ec3f7dd03925ae8.nq.gz
    ├── 159d651a5b6d26fc6342ba7745eb06d3c8f5fdd7.nq.gz
    ├── 15a17790d99340f3c397c1fb17d776afc05ea750.nq.gz
    ├── 15a50506cfce4e8d5410aec84075da97bc870d9c.nq.gz
    ├── 15c9699ec4d129263f2592c9f39b9f34e31f95c6.nq.gz
    ├── 15e338fc1117b6cbd88fd09bd1759fb806973e3d.nq.gz
    ├── 165e937eba63a1f795c6fc2946ac4c3c539acd1d.nq.gz
    ├── 1691a8c03f4af3e295eca60fda0d132f99871e30.nq.gz
    ├── 16ba717b681febcb718863db08dd23fba92d2c26.nq.gz
    ├── 1701e7f25681ef5317c6e73d410bdfa74f76775e.nq.gz
    ├── 170e974c15746c3aa6e960d3c7a53981459a528d.nq.gz
    └── 171dae4424ca171f9f3cf48781387571f4e5cdb2.nq.gz

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
*Parsed on 2026-03-21 by [repolex](https://repolex.ai)*
