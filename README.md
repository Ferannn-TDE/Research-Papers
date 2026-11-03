# CS434 Research Papers: Machine Learning for Database Systems

A collection of research papers on learned query optimization, join order
selection, and query plan representation. Four papers are included as PDFs; two
are available through external links while redistribution permission is pending.
The index provides citations and official sources for all six papers.

This repository contains research PDFs, this reading guide, and Git file rules.
It contains no original implementations, notebooks, datasets, trained models,
experiments, or reproduced results. The two excluded PDFs remain unchanged on
the maintainer's computer.

## Paper index

### 1. Efficient Join Order Selection Learning with Graph-based Representation

**Authors:** Jin Chen, Guanyu Ye, Yan Zhao, Shuncheng Liu, Liwei Deng, Xu Chen,
Rui Zhou, and Kai Zheng.

**Publication:** 2022. *Proceedings of the 28th ACM SIGKDD Conference on Knowledge
Discovery and Data Mining* (KDD '22), pp. 97–107.

**Official links:** [DOI: 10.1145/3534678.3539303](https://doi.org/10.1145/3534678.3539303)
and [KDD 2022 proceedings entry](https://kdd.org/kdd2022/toc.html).
The proceedings page lists the paper under its full title.

**Repository copy:** External links only. `efficient_join.pdf` is excluded because
its ACM notice requires permission for posting on servers, and that permission
has not been established.

**Focus:** JOGGER uses graph representations and curriculum learning for join
order selection.

### 2. Graph Neural Networks for Databases: A Survey

**Authors:** Ziming Li, Youhuan Li, Yuyu Luo, Guoliang Li, and Chuxu Zhang.

**Publication:** 2025. *Proceedings of the Thirty-Fourth International Joint
Conference on Artificial Intelligence* (IJCAI-25), Survey Track, pp. 10555–10563.

**Official link:** [IJCAI publication page](https://ijcai.org/proceedings/2025/1172).
DOI: `10.24963/ijcai.2025/1172`.

**Repository copy:** [graph_neural_networks.pdf](graph_neural_networks.pdf).

**Focus:** A survey of graph neural network applications in relational and graph
databases.

### 3. LOGER: A Learned Optimizer towards Generating Efficient and Robust Query Execution Plans

**Authors:** Tianyi Chen, Jun Gao, Hedui Chen, and Yaofeng Tu.

**Publication:** 2023. *Proceedings of the VLDB Endowment* (PVLDB), 16(7),
pp. 1777–1789.

**Official link:** [VLDB publisher PDF](https://www.vldb.org/pvldb/vol16/p1777-gao.pdf).
DOI: `10.14778/3587136.3587150`.

**Repository copy:** [learned_optimizer.pdf](learned_optimizer.pdf), under the
CC BY-NC-ND 4.0 notice printed in the paper.

**Focus:** Learned join ordering and physical operator restrictions for robust
query plan generation.

### 4. Neo: A Learned Query Optimizer

**Authors:** Ryan Marcus, Parimarjan Negi, Hongzi Mao, Chi Zhang, Mohammad
Alizadeh, Tim Kraska, Olga Papaemmanouil, and Nesime Tatbul.

**Publication:** 2019. *Proceedings of the VLDB Endowment* (PVLDB), 12(11),
pp. 1705–1718.

**Official link:** [VLDB publisher PDF](https://www.vldb.org/pvldb/vol12/p1705-marcus.pdf).
DOI: `10.14778/3342263.3342644`.

**Repository copy:** [learned_theory_optimizer.pdf](learned_theory_optimizer.pdf),
under the CC BY-NC-ND 4.0 notice printed in the paper.

**Focus:** Neural query optimization that learns from execution feedback.

### 5. Reinforcement Learning with Tree-LSTM for Join Order Selection

**Authors:** Xiang Yu, Guoliang Li, Chengliang Chai, and Nan Tang.

**Publication:** 2020. *2020 IEEE 36th International Conference on Data Engineering*
(ICDE), pp. 1297–1308.

**Official link:** [IEEE Computer Society proceedings PDF](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300b297/290300b297.pdf).
DOI: `10.1109/ICDE48307.2020.00116`.

**Repository copy:** External link only. `reinforcemnet_learning.pdf` is excluded
until permission for third-party reposting is established under IEEE's posting
policy. No open redistribution license was found in the local PDF.

**Focus:** RTOS combines tree representations and reinforcement learning for join
order selection.

### 6. QueryFormer: A Tree Transformer Model for Query Plan Representation

**Authors:** Yue Zhao, Gao Cong, Jiachen Shi, and Chunyan Miao.

**Publication:** 2022. *Proceedings of the VLDB Endowment* (PVLDB), 15(8),
pp. 1658–1670.

**Official link:** [VLDB publisher PDF](https://www.vldb.org/pvldb/vol15/p1658-zhao.pdf).
DOI: `10.14778/3529337.3529349`.

**Repository copy:** [tree_transformer.pdf](tree_transformer.pdf), under the
CC BY-NC-ND 4.0 notice printed in the paper.

**Focus:** Tree-structured Transformers for query plan encoding.

## Verification and access

Citation details were checked on 2026-11-02 against the local PDFs and the
official KDD, IJCAI, VLDB, and IEEE Computer Society sources linked above. Author
order follows the published reference blocks or publisher records, rather than
the order returned by text extraction from multi-column page layouts.

The local RTOS PDF does not show its publication year, venue, or DOI on its first
page; those details were verified in the IEEE proceedings PDF. No citation fields
remain unverified.

The ACM Digital Library landing page for JOGGER returned HTTP 403 to the automated
checker. Its DOI matches the local PDF and the link in the official KDD
proceedings entry; the KDD entry was accessible. The other five official source
links were accessible during verification. Publisher access policies may differ
for individual readers.

## Repository contents and reading the PDFs

| Path | Role | Included in Git? |
| --- | --- | --- |
| `README.md` | Paper citations, reading guide, and scope | Yes |
| `.gitignore` | Two specific paper exclusions and operating system metadata exclusions | Yes |
| `.gitattributes` | Keeps PDFs binary, without text conversion or text diffs | Yes |
| `efficient_join.pdf` | JOGGER, 11 pages; permission pending | No; external links only |
| `graph_neural_networks.pdf` | GNN survey, 9 pages | Yes |
| `learned_optimizer.pdf` | LOGER, 13 pages | Yes |
| `learned_theory_optimizer.pdf` | Neo, 14 pages | Yes |
| `reinforcemnet_learning.pdf` | RTOS, 12 pages; permission pending | No; external link only |
| `tree_transformer.pdf` | QueryFormer, 13 pages | Yes |

All six original PDFs are preserved locally without changes. Only JOGGER and
RTOS are ignored by Git. The other four PDFs are selected for inclusion in the
public repository. Original filenames are unchanged, including the spelling of
`reinforcemnet_learning.pdf`.

Use the repository PDF links in the index to read the four included papers on
GitHub. Use the official online links for the two excluded papers. As an optional
way to read a downloaded copy on macOS, run this command from the project folder:

```sh
open graph_neural_networks.pdf
```

This command opens the survey and generates no project output. Reading requires
only a browser or PDF reader; there are no dependencies to install,
environment variables to configure, build steps, or automated tests.

## Data and reproducibility

The papers discuss benchmarks such as JOB, TPC-H, and TPC-DS. Their datasets,
database setup, training code, and experiment configurations are not included in
this collection. Reproducing a paper's experiments requires the corresponding
authors' implementations, data, and instructions. This repository has no data
processing pipeline and generates no reports, figures, or model checkpoints.
The papers' experimental results have not been reproduced or independently
verified here.

## Licensing

The papers retain their original copyrights and terms. This repository does not
assign a new license to third-party material. Citations, authors, and official
source links are provided in the index. The included PDFs are the existing local
copies, unchanged by this repository preparation, with their original notices
retained.

| File | Redistribution basis or remaining issue |
| --- | --- |
| `graph_neural_networks.pdf` | Copyright holder: [IJCAI Organization](https://ijcai.org/contact/). Its proceedings policy permits republishing with a visible reference and link to IJCAI; both are provided above and here. |
| `learned_optimizer.pdf` | The paper states CC BY-NC-ND 4.0; included with attribution for noncommercial sharing without adaptations. |
| `learned_theory_optimizer.pdf` | The paper states CC BY-NC-ND 4.0; included with attribution for noncommercial sharing without adaptations. |
| `tree_transformer.pdf` | The paper states CC BY-NC-ND 4.0; included with attribution for noncommercial sharing without adaptations. |
| `efficient_join.pdf` | Excluded: its ACM notice requires permission for posting on servers. Permission has not been established. |
| `reinforcemnet_learning.pdf` | Excluded: no open redistribution license was found in the local copy, and IEEE's conference-paper posting policy requires permission for third-party reuse. Permission has not been established. |

The three VLDB papers retain their existing
[CC BY-NC-ND 4.0 terms](https://creativecommons.org/licenses/by-nc-nd/4.0/): credit
the authors, retain the license link and notices, use them only for noncommercial
purposes, and do not distribute adaptations. RTOS remains linked to the official
publisher copy under
[IEEE's conference-paper posting policy](https://conferences.ieeeauthorcenter.ieee.org/get-published/post-your-paper/).
The IJCAI and IEEE policy pages were checked on 2026-11-02.

No license has been selected for the original documentation. Choosing a license
for that documentation is an optional future decision for the repository owner.
