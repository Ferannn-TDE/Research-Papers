# CS434 Reading List: Machine Learning for Database Systems

A reading list of six research papers on learned query optimization, join order
selection, and query plan representation. Follow the official online links below
to browse the papers without needing local files.

This repository contains the reading guide and Git ignore rules. It contains no
original implementations, notebooks, datasets, trained models, experiments, or
reproduced results. Optional local PDF copies are kept outside Git.

## Paper index

### 1. Efficient Join Order Selection Learning with Graph-based Representation

**Authors:** Jin Chen, Guanyu Ye, Yan Zhao, Shuncheng Liu, Liwei Deng, Xu Chen,
Rui Zhou, and Kai Zheng.

**Publication:** 2022. *Proceedings of the 28th ACM SIGKDD Conference on Knowledge
Discovery and Data Mining* (KDD '22), pp. 97–107.

**Official links:** [DOI: 10.1145/3534678.3539303](https://doi.org/10.1145/3534678.3539303)
and [KDD 2022 proceedings entry](https://kdd.org/kdd2022/toc.html).
The proceedings page lists the paper under its full title.

**Focus:** JOGGER uses graph representations and curriculum learning for join
order selection.

### 2. Graph Neural Networks for Databases: A Survey

**Authors:** Ziming Li, Youhuan Li, Yuyu Luo, Guoliang Li, and Chuxu Zhang.

**Publication:** 2025. *Proceedings of the Thirty-Fourth International Joint
Conference on Artificial Intelligence* (IJCAI-25), Survey Track, pp. 10555–10563.

**Official link:** [IJCAI publication page](https://ijcai.org/proceedings/2025/1172).
DOI: `10.24963/ijcai.2025/1172`.

**Focus:** A survey of graph neural network applications in relational and graph
databases.

### 3. LOGER: A Learned Optimizer towards Generating Efficient and Robust Query Execution Plans

**Authors:** Tianyi Chen, Jun Gao, Hedui Chen, and Yaofeng Tu.

**Publication:** 2023. *Proceedings of the VLDB Endowment* (PVLDB), 16(7),
pp. 1777–1789.

**Official link:** [VLDB publisher PDF](https://www.vldb.org/pvldb/vol16/p1777-gao.pdf).
DOI: `10.14778/3587136.3587150`.

**Focus:** Learned join ordering and physical operator restrictions for robust
query plan generation.

### 4. Neo: A Learned Query Optimizer

**Authors:** Ryan Marcus, Parimarjan Negi, Hongzi Mao, Chi Zhang, Mohammad
Alizadeh, Tim Kraska, Olga Papaemmanouil, and Nesime Tatbul.

**Publication:** 2019. *Proceedings of the VLDB Endowment* (PVLDB), 12(11),
pp. 1705–1718.

**Official link:** [VLDB publisher PDF](https://www.vldb.org/pvldb/vol12/p1705-marcus.pdf).
DOI: `10.14778/3342263.3342644`.

**Focus:** Neural query optimization that learns from execution feedback.

### 5. Reinforcement Learning with Tree-LSTM for Join Order Selection

**Authors:** Xiang Yu, Guoliang Li, Chengliang Chai, and Nan Tang.

**Publication:** 2020. *2020 IEEE 36th International Conference on Data Engineering*
(ICDE), pp. 1297–1308.

**Official link:** [IEEE Computer Society proceedings PDF](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300b297/290300b297.pdf).
DOI: `10.1109/ICDE48307.2020.00116`.

**Focus:** RTOS combines tree representations and reinforcement learning for join
order selection.

### 6. QueryFormer: A Tree Transformer Model for Query Plan Representation

**Authors:** Yue Zhao, Gao Cong, Jiachen Shi, and Chunyan Miao.

**Publication:** 2022. *Proceedings of the VLDB Endowment* (PVLDB), 15(8),
pp. 1658–1670.

**Official link:** [VLDB publisher PDF](https://www.vldb.org/pvldb/vol15/p1658-zhao.pdf).
DOI: `10.14778/3529337.3529349`.

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

## Contents and optional local reading

| Path | Role | Included in Git? |
| --- | --- | --- |
| `README.md` | Paper citations, reading guide, and scope | Yes |
| `.gitignore` | Exact PDF exclusions and operating system metadata exclusions | Yes |
| `efficient_join.pdf` | Local JOGGER copy, 11 pages | No |
| `graph_neural_networks.pdf` | Local GNN survey copy, 9 pages | No |
| `learned_optimizer.pdf` | Local LOGER copy, 13 pages | No |
| `learned_theory_optimizer.pdf` | Local Neo copy, 14 pages | No |
| `reinforcemnet_learning.pdf` | Local RTOS copy, 12 pages | No |
| `tree_transformer.pdf` | Local QueryFormer copy, 13 pages | No |

The six existing PDFs are preserved locally and ignored by Git. A clone of this
repository will not include them. Original filenames are unchanged, including
the spelling of `reinforcemnet_learning.pdf`.

If you already have the local copies, open them with any PDF reader. For example,
from this folder on macOS:

```sh
open efficient_join.pdf
```

This optional command opens the local paper and generates no project output.
Online reading requires only a browser; there are no dependencies to install,
environment variables to configure, build steps, or automated tests.

## Data and reproducibility

The papers discuss benchmarks such as JOB, TPC-H, and TPC-DS. Their datasets,
database setup, training code, and experiment configurations are not included in
this reading list. Reproducing a paper's experiments requires the corresponding
authors' implementations, data, and instructions. This repository has no data
processing pipeline and generates no reports, figures, or model checkpoints.
The papers' experimental results have not been reproduced or independently
verified here.

## Licensing

Third-party papers are linked from their official sources and are not distributed
by this repository. Their copyrights and license terms remain with their
respective rights holders; no license is assigned to them here.

No license has been selected for the original documentation. Choosing a license
for that documentation is an optional future decision for the repository owner.
