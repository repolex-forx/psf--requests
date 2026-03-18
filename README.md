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
│   │   ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│   │   ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│   │   ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│   │   ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│   │   ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│   │   ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│   │   ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│   │   ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│   │   ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   └── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   ├── dataflow
│   │   ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│   │   ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│   │   ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│   │   ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│   │   ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│   │   ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│   │   ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│   │   ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│   │   ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│   │   ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│   │   ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   └── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   ├── lsp
│   │   ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│   │   ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│   │   ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│   │   ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│   │   ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│   │   ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│   │   ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│   │   ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│   │   ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│   │   ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│   │   ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│   │   ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│   │   ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│   │   ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│   │   └── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
│   └── repolex
│       ├── 082f4d89486e4bfe918fd125431545a6b879155e.nq.gz
│       ├── 0c00a17372891f6cfee91d1b5ab5cb632a3b52ef.nq.gz
│       ├── 1a7c91f6581c80122ed8cd1fdf4a8ca38c842453.nq.gz
│       ├── 1be2a55a39b0738c7e07f3bd356306de2683f04e.nq.gz
│       ├── 5b5ff6920102e013cf041bd342459e4e0613294f.nq.gz
│       ├── 63243b1e3b435c7736acf1e51c0f6fa6666d861d.nq.gz
│       ├── 6562137731f9ad11be7c156fa25220fc3a7ffe03.nq.gz
│       ├── 775b6f6f0098ffa9edd3874b1af4b98378377211.nq.gz
│       ├── 8c90c610cd15f91ed0cd1738aa73f088496b6af9.nq.gz
│       ├── 95ba6fcab2564a0e13f7fec99e4470a851b19c99.nq.gz
│       ├── add6feab02d21967ca35f1572e6202b1dd11b788.nq.gz
│       ├── bca920c1c1a96e191ec7f9fcaec5f53e46edf08e.nq.gz
│       ├── c18e6459a80d83c54f787549565eedb3a0210156.nq.gz
│       ├── d2cdefa7df40e8b9cb98e831dc70bcefa71467c5.nq.gz
│       └── d938f3208968949decbb0a21292deb1451c211d5.nq.gz
└── blob
    ├── 0063935ce65a9adb52e1504f0783366f355c0b85.nq.gz
    ├── 00b2cd58c891fb121a1f4b02a1557fa906a95e78.nq.gz
    ├── 01c10638ede3992a41d55c1302c26bf81acecfc1.nq.gz
    ├── 0417d6f668c9ae16897ef4d1c80fb5664110a452.nq.gz
    ├── 04f2d7fb4405bb013f12b40692ecb20974fab359.nq.gz
    ├── 0546a121a5830e5382f7deba37985be1e5172f66.nq.gz
    ├── 055154d01a949305b629905c16454c40f820e024.nq.gz
    ├── 063d5f96a8aff4906b0cb9864d48718b7bdc58b6.nq.gz
    ├── 064345b0867d4d23ef17a4d7d11663dcf3cf4adf.nq.gz
    ├── 07698f6f6ee89a319bf32d0be6089238002c665e.nq.gz
    ├── 0820d59c379e055c0a4a1c52adb0aaa8128cbb15.nq.gz
    ├── 08ba2bc6f12d8e9a61e175a366fe0261de84a52f.nq.gz
    ├── 08edab4e17fb773bc60bf3bba98b0e095cc67a4e.nq.gz
    ├── 09b549014ccde6ef78029c2cb08b317a1121add9.nq.gz
    ├── 0ace12b6964c0cff7772ce959dc691b3831f56c7.nq.gz
    ├── 0adfa0f5d174c49b7c09ee20388d407f010cbf58.nq.gz
    ├── 0ae2182eb19880acda28f4ee8b0ab4cf4b671025.nq.gz
    ├── 0b725cae94caf79feaedca0d5ea16578888b27d2.nq.gz
    ├── 0c82c7b46f7664c42031fb85f7355c995aad76d5.nq.gz
    ├── 0cda6591ae53896dfd866da5ab00030513064456.nq.gz
    ├── 0e0405ce3afd69dd9653276e6edf91e09aba4ea1.nq.gz
    ├── 0e0dd67f649def8d0eb44a653148883867ac4464.nq.gz
    ├── 0e274101cd5933b4e5408efbf1e6ab8709b77932.nq.gz
    ├── 0e7836db1c23062596e1690dcab11dc47f3d2789.nq.gz
    ├── 0e80eaa24a24a9f60546b1962af368e0783ef5af.nq.gz
    ├── 0e8933cf1edb7bd1fc34b79970aa346891cdd6b7.nq.gz
    ├── 0eb7b2f31de03f0c61e5bc633287b7d10b0121b7.nq.gz
    ├── 0f6d9ca93717e81aced697a57d10da8ac547ec97.nq.gz
    ├── 0fb8d7052adcb894d940db7874e633ed934dfcdb.nq.gz
    ├── 101d1ce6007eb1e6d2e357f76be1fa91231508a2.nq.gz
    ├── 1140a523f59bca36cffedab8af8d18eb34e03743.nq.gz
    ├── 1238f510fc6afe2739f3f7a44359cfe471c154a3.nq.gz
    ├── 124458818d77f3e410d89f0aa9caf96f3d8c46f7.nq.gz
    ├── 12db07cd00038169e9a0844a1e6d663d8fa43e1d.nq.gz
    ├── 12e1fd77ff1ef7b4ac198c7002f7d9a500cc5a99.nq.gz
    ├── 131c0f61c7e06072e040d52b5c0a9695f851d864.nq.gz
    ├── 139334ab6660f597c44c2b4d741e4b72ed72d46b.nq.gz
    ├── 13d0eb5c25ebda4328398ffa971efa311be4d2bb.nq.gz
    ├── 145838f2009ea1228c8d71dcac37636fbd173cb1.nq.gz
    ├── 1463fa1d85c86785b16efc6663602ff736105cae.nq.gz
    ├── 1473d1258b24a3bd0d024026af3f81938b6a6a86.nq.gz
    ├── 1507609a6b58675b8cf9c10e5ec3f7dd03925ae8.nq.gz
    ├── 159d651a5b6d26fc6342ba7745eb06d3c8f5fdd7.nq.gz
    ├── 15a17790d99340f3c397c1fb17d776afc05ea750.nq.gz
    ├── 15a50506cfce4e8d5410aec84075da97bc870d9c.nq.gz
    ├── 15c9699ec4d129263f2592c9f39b9f34e31f95c6.nq.gz
    ├── 165e937eba63a1f795c6fc2946ac4c3c539acd1d.nq.gz
    ├── 1691a8c03f4af3e295eca60fda0d132f99871e30.nq.gz
    ├── 171dae4424ca171f9f3cf48781387571f4e5cdb2.nq.gz
    ├── 17e503a2262a9a0880eea32fc99b6fba89b2af8d.nq.gz
    ├── 17f2f847e984c585f1bae5c7f192199b8a4ad4d6.nq.gz
    ├── 183d475ab9ad506152f6318deb7c6c8c88ee5a79.nq.gz
    ├── 186609054f744131dba3bfe07977653684076a14.nq.gz
    ├── 19d0e4c08c3cd5a20cf89245e6fd49f93e155375.nq.gz
    ├── 1ab216b1c4fc27cb11abae1876c8b125822bae71.nq.gz
    ├── 1b591d4b54dadc7c288003d24714d627d845fdd0.nq.gz
    ├── 1b847b7bb6d59b9741849dbdf6301be027a4e91c.nq.gz
    ├── 1bda9ff1620fe71ad78425112af48e21a14f52ef.nq.gz
    ├── 1c6df309edc8fd9c5aaa21d4a7fb867dd73ba8ec.nq.gz
    ├── 1c88f564ccda34565ddeb5e967964a6ef7f1fece.nq.gz
    ├── 1cf3aa6db6d938b571af5f4ca6cb397fcc73dace.nq.gz
    ├── 1cffa805c52f7ba72326a3f5fc895c6f424da6c9.nq.gz
    ├── 1d2826168923c2ce71f96d15b909e77b15ae8250.nq.gz
    ├── 1d335f420a2193fd8a0ebef837cf9b0c08b7fe9e.nq.gz
    ├── 1d6716df9cd9dd5b19a2e71348c287d0e6fe627b.nq.gz
    ├── 1d842e6e7adf14fd7406e1f675e0504db5abf23b.nq.gz
    ├── 1db8611d8d1d0517a8c1cc14f61e7c29d7c2cac7.nq.gz
    ├── 1e4d89b0717bba048be5df666aeed573b1da8e47.nq.gz
    ├── 1eee253c047ec52c4eb6b473a4f3e3e816a034cf.nq.gz
    ├── 1f466886a63046b2430a262ebf4a0e9b3e80b097.nq.gz
    ├── 1ffd778d739ae60f378ba52b52bc7f5d1601f99b.nq.gz
    ├── 208803a771673d888bbd08f57d1767da60fe3242.nq.gz
    ├── 20b1fb4ea7dc9a2e4155df072543845a60db521d.nq.gz
    ├── 216367a0c757883b7f11b692f0c947687758d76b.nq.gz
    ├── 219862477a8ca158b1bb515ecf19cc3af5b999aa.nq.gz
    ├── 232d6830461717a1065e6c1ebb0ef398c831062f.nq.gz
    ├── 24b77a6dae0a466611be49937788128facba1dde.nq.gz
    ├── 26335e5d6bcaea548c8dbcd2b1a53debc12428e6.nq.gz
    ├── 2684a2fd402097457c3b9c62b5423357b8838873.nq.gz
    ├── 26f01767b9ea7b144494511deea745f09a7292e4.nq.gz
    ├── 277e6010d4a51318b4f845c76b601146f17ec9b2.nq.gz
    ├── 27d80112bf93d3d782bb1b5ced6f8ca7bd7285a3.nq.gz
    ├── 280977dafac2597448d5f504284b3c8a6e95df6a.nq.gz
    ├── 28537d3b628225bbb027c1ce7322ceb35b7271af.nq.gz
    ├── 292e8af7691259f79fc0f8cb196f32a121676690.nq.gz
    ├── 2938029b6c06aea1f85ccf0f33c4b17da28b60c7.nq.gz
    ├── 29596547489c1c413459127ca91d32bd238e65d0.nq.gz
    ├── 29c06c6baacb44a06c7600133249fbd188bc397d.nq.gz
    ├── 2a9208cc50851386c6d217688374b7362439314c.nq.gz
    ├── 2ad08f0f92ec413b610bf8ced13d407e4a1166c5.nq.gz
    ├── 2b4704e81f42aabea3b7517bfff5ca98cc6ab1e7.nq.gz
    ├── 2b9ba77bcce8c6a1a70cc05a73c744860281371f.nq.gz
    ├── 2bf6e11dd8f122a7d59eaa19ff23d4ddfaa4e387.nq.gz
    ├── 2c3241d4ae98f04a48e4f60d1a1a8689138f95e0.nq.gz
    ├── 2c63061d1dba047614d4ca81b28b02338f045793.nq.gz
    ├── 2cf901631d0d623e8f101ad6219cf3f882b87d00.nq.gz
    ├── 2d37bbb0bd80e56a58870a920ddc9103116dd23f.nq.gz
    ├── 2d6fecec4f024933fd026d852f45ccaa420b3f0a.nq.gz
    ├── 2da09824af81e5ecf08f0d8115fa2fe3f0fea0bb.nq.gz
    ├── 2dc0b31246ae6b1e91ef6ace195c6d6686ef6e21.nq.gz
    ├── 2e16163bf60c13ec25da998d683ac10140d607fe.nq.gz
    ├── 2e2bebcb2ba9d72762f16cfa5377941ef0ff3a81.nq.gz
    ├── 2e7b471532fcba9c4ba5dd1ce175139eeec798b6.nq.gz
    ├── 2e875d46ea40c602c75394acb8d4608705b52cbb.nq.gz
    ├── 2e96919c645725b90c5dcb4644e72f84812cd4c0.nq.gz
    ├── 2e9c663ea519baf1bf0c80e0e32ba6053cf9acd0.nq.gz
    ├── 2ffea8bbf504f6f1f4d0012d31e3c100411e487a.nq.gz
    ├── 307a1f0d658343ab2579dffd080f035a94a7e87f.nq.gz
    ├── 307d4845b4601b092f4e4dd27722aaff332b4a61.nq.gz
    ├── 310ea21d96a7e5f6c8828b3031ade3f0b0c1de56.nq.gz
    ├── 318691f0d3c42fa464f232d52cf63226c8f51ab7.nq.gz
    ├── 3202ee67549148c0079046423faf144ae5f829a4.nq.gz
    ├── 336aa7737edaeae1dd3073f72b5a044994b8de1a.nq.gz
    ├── 33f47449c11d241e36c83d7f95d819bbe56e2c8f.nq.gz
    ├── 344a1030ccce046fd36f8802121e4bb763294f22.nq.gz
    ├── 347411748250982eb59a8f3937dc059de1e99dd9.nq.gz
    ├── 349e9c457025d6f737f057d00f7b62898d800883.nq.gz
    ├── 3560b89de710e43a8bdaed54d185ae58d44d7df9.nq.gz
    ├── 358dfce69b71bb41ddbf9cc115429699de47728c.nq.gz
    ├── 359d74476a248528208481a57b7bcfdff2bb8660.nq.gz
    ├── 35a903fd33ec255c3f153bf7967187fbffade2a0.nq.gz
    ├── 362463100e935a91120aed487232381980ce6437.nq.gz
    ├── 36d47f7c9871e8ea17131cfea37b17b8ecdd5339.nq.gz
    ├── 37063f584b360f3a4c178fc0bf51286761ec3434.nq.gz
    ├── 37467542075fe028c3e02da79b4c144e5d1c64bd.nq.gz
    ├── 375bd9d983f597a61fc38405f62d7e49674a1955.nq.gz
    ├── 379d769d48931d3b0be8d5ab5ea7951a14505983.nq.gz
    ├── 37d964cf802704a5837a7555883af5af42eb84b8.nq.gz
    ├── 37e8351577681ea1ea7a116a7d719adb4de5025d.nq.gz
    ├── 37f87d939944ac53dc087a32df3a96d23fd435c1.nq.gz
    ├── 385dd27d0cc4edb3d89e10fda648993849528d51.nq.gz
    ├── 38e5bc61b55e4c50a7b3de8b49973a49ff050b29.nq.gz
    ├── 39e652ed44ecba5fc42b5a08338debc3905b264d.nq.gz
    ├── 39fbb99463cffef1d3d7a0c8cc144df96399860d.nq.gz
    ├── 3a13c358819811ac032ad39b0f78aac2cc0288f6.nq.gz
    ├── 3a5a762eb565729508803aeb238180d900e6ce8a.nq.gz
    ├── 3a720c9a9af8ebdf437b706edd53ac18e1f6670d.nq.gz
    ├── 3abfe7b8bbc4be26c736e42b0726ebafd6c471c0.nq.gz
    ├── 3ac1683c7912c4f7afb5778d671a2127914772c9.nq.gz
    └── 3c074d1be9d209eaef0bec661912eaa0b4f5aa94.nq.gz

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
*Parsed on 2026-03-18 by [repolex](https://repolex.ai)*
