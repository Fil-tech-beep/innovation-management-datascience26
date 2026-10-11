# Patent analytics on TIP · Innovation Management 2026/27

Tutorials for the **Project Work (PW)** of the *Innovation Management* course, MSc in **Data Science and Engineering**, Politecnico di Torino, academic year 2026/27.

The notebooks run on the **EPO Technology Intelligence Platform (TIP)** and use **PATSTAT** to turn patent data into a description of a technology sector. They assume you can program in Python and SQL, but **no prior knowledge of patent data**.

## Contents

### Tutorial 0 · Getting started with TIP and PATSTAT

| # | Notebook | What you learn | PW step | Time |
|---|---|---|---|---|
| 00 | [TIP platform](tutorial_0/00_tip_platform.ipynb) | JupyterLab on TIP, terminal, resource limits, available data | basic knowledge | 15 min |
| 01 | [PATSTAT basics](tutorial_0/01_patstat_basics.ipynb) | PATSTAT schema, ORM and raw SQL queries, building a sector dataset | Step 0 · data collection | 30 min |
| 02 | [General description of the sector](tutorial_0/02_step1_general_description.ipynb) | Families vs applications, which year to use, growth, technology mix, geography | Step 1 · general description | 30 min |

Work through them **in order**: each notebook builds on the previous one.

## How to get the notebooks on TIP

**Option A, with Git (recommended).** Open a terminal on TIP (*File → New → Terminal*) and run:

```bash
git clone https://github.com/graziasveva/innovation-management-datascience26.git
```

When the material is updated during the course, get the new version with:

```bash
cd innovation-management-datascience26
git pull
```

> Work on a **copy** of each notebook (right-click → *Duplicate*, e.g. `02_step1_general_description_myteam.ipynb`), so that `git pull` never conflicts with your changes.

**Option B, without Git.** Download the zip from the [Releases](../../releases) page, then upload it to TIP and unzip it from the terminal with `unzip innovation-management-datascience26-v1.0.zip`.

## Working rules

- Develop on the **TEST** environment (`ENV = "TEST"`), a small subset of PATSTAT. Switch to **PROD** only to produce your final numbers: it is the full database and is much slower.
- Run each notebook from top to bottom (*Kernel → Restart Kernel and Run All Cells*) before trusting its results.
- Keep the aggregation inside the database: download small result tables, never millions of rows.

## Repository structure

```
innovation-management-datascience26/
├── README.md
├── LICENSE.md                  terms of use and attribution
└── tutorial_0/
    ├── 00_tip_platform.ipynb
    ├── 01_patstat_basics.ipynb
    ├── 02_step1_general_description.ipynb
    └── img/                    screenshots used by the notebooks
```

## Acknowledgements

This material is based on the **EPO TIP training materials** published by the European Patent Office at <https://github.com/epo/tip-training>. It has been **tailored and enriched** for the students of the MSc in Data Science and Engineering (2026, Innovation Management class) at Politecnico di Torino.

This is a **modified version** of the original EPO material. It **has not been authorised by the EPO**, and the EPO is not responsible for the correctness of this modified version. See [LICENSE.md](LICENSE.md).

## Contact

Prof. Grazia Sveva Ascione · Politecnico di Torino · questions about the PW: during the course tutorials or by e-mail.

_Version 1.0 · October 2026_
