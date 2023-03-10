# โ๏ธ FIERLENIUS ๐ฆ

โ Authors:

**ROUAUD Lucas**

Master 2 Bio-informatics at *Univeritรฉ de Paris*

[![Python 3.10.8](https://img.shields.io/badge/python-%E2%89%A5_3.10.8-blue.svg)](https://www.python.org/downloads/release/python-397/)
[![Conda 22.11.1](https://img.shields.io/badge/miniconda-%E2%89%A5_22.11.1-green.svg)](https://docs.conda.io/en/latest/miniconda.html)
[![GitHub last commit](https://img.shields.io/github/last-commit/FilouPlains/FIERLENIUS.svg)](https://github.com/FilouPlains/FIERLENIUS)
![GitHub stars](https://img.shields.io/github/stars/FilouPlains/FIERLENIUS.svg?style=social)


## ๐งฎ Dataset origin

- **`SCOPe_2.08_classification.txt` :**
    - Extract from the `SCOPe 2.08` database, download the `01/2023`. Contains the classifications with the category. Only globular domains are kept.
- **`SCOPe_2.08_95identity_globular.fasta` :**
    - Extract from the `SCOPe 2.08` database, download the `02/2023`. Contains the classified sequences. Only globular domains are kept.
- **`pyHCA_SCOPe_30identity.out` :**
    - Extract from this Github repository: [DarkVador-HCA/Order-Disorder-continuum/blob/main/data/SCOPe/hca.out](https://github.com/DarkVador-HCA/Order-Disorder-continuum/blob/main/data/SCOPe/hca.out).
- **`HCDB_2018_summary_rss.csv` :**
    - Local database, version `02/2018`.
- **`peitsch2vec/` :**
    - Generate data with the script [`src/embeddings/peitsch2vec.py`](src/embeddings/peitsch2vec.py). In `peitsch2vec/default_domain/`, data have been generated without the option `--segment`, while in `peitsch2vec/default_segments/`, data have been generated with the option `--segment`.

## ๐ฒ Dependencies tree

```bash
$ tree -lF -h
.
โโโ [4.0K]  "data/"
โย ย  โโโ [ 15M]  "dir.des.scope.2.08-stable.txt"
โย ย  โโโ [4.4M]  "hca.out"
โย ย  โโโ [4.6K]  "HCDB_summary.csv"
โย ย  โโโ [4.0K]  "peitsch2vec/"
โย ย      โโโ [4.0K]  "default_domain/"
โย ย      โย ย  โโโ [ 26K]  "characteristics_2023-02-14_15-40-13.npy"
โย ย      โย ย  โโโ [762K]  "embedding_2023-02-14_15-40-13.npy"
โย ย      โย ย  โโโ [413K]  "matrix_cosine_2023-02-14_15-40-13.npy"
โย ย      โย ย  โโโ [776K]  "model_2023-02-14_15-40-13.w2v"
โย ย      โโโ [4.0K]  "default_segments/"
โย ย          โโโ [ 26K]  "characteristics_2023-02-14_15-40-13.npy"
โย ย          โโโ [762K]  "embedding_2023-02-14_15-40-13.npy"
โย ย          โโโ [413K]  "matrix_cosine_2023-02-14_15-40-13.npy"
โย ย          โโโ [776K]  "model_2023-02-14_15-40-13.w2v"
โโโ [4.0K]  "docs/"
โย ย  โโโ [4.0K]  "embedding/"
โย ย  โย ย  โโโ [5.0M]  "comparing_distribution.html"
โย ย  โย ย  โโโ [8.6M]  "matrix.html"
โย ย  โย ย  โโโ [5.0M]  "projection.html"
โย ย  โโโ [ 15K]  "index.html"
โย ย  โโโ [7.2K]  "jupyter_logo_icon.svg"
โย ย  โโโ [2.3K]  "style.css"
โย ย  โโโ [4.0K]  "svg/"
โย ย      โโโ [ 27K]  "CBOW.svg"
โย ย      โโโ [2.2K]  "context_scheme.svg"
โย ย      โโโ [5.1K]  "domain_to_peitsch.svg"
โโโ [4.0K]  "env/"
โย ย  โโโ [ 369]  "fierlenius.yml"
โย ย  โโโ [ 740]  "README.md"
โโโ [1.5K]  "README.md"
โโโ [4.0K]  "src/"
    โโโ [4.0K]  "embeddings/"
    โย ย  โโโ [6.6K]  "arg_parser.py"
    โย ย  โโโ [3.3K]  "domain.py"
    โย ย  โโโ [2.2K]  "hca_reader.py"
    โย ย  โโโ [1.1K]  "hcdb_parser.py"
    โย ย  โโโ [4.0K]  "notebook/"
    โย ย  โย ย  โโโ [6.6M]  "comparing_distribution.ipynb"
    โย ย  โย ย  โโโ [ 15M]  "matrix.ipynb"
    โย ย  โย ย  โโโ [5.8M]  "projection.ipynb"
    โย ย  โย ย  โโโ [6.3K]  "sammon.py"
    โย ย  โโโ [7.4K]  "peitsch2vec.py"
    โย ย  โโโ [4.8K]  "peitsch.py"
    โโโ [4.0K]  "msa/"
```
