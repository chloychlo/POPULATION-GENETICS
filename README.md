# Population Genetics Simulation

## Project Overview 

This project implements a stochastic simulator to investigate fundamental mechanisms of molecular evolution and population genetics. 

The primary goal is to bridge theoretical derivations from population genetics lectures with computational experiments across replicated populations, verifying statistical predictions regarding allele frequency dynamics, genetic diversity, and fixation probabilities.

### Model Assumptions
* **Population Structure**: $N$ haploid (or diploids), asexually (or sexually) reproducing individuals with discrete, non-overlapping generations.
* **Genome Architecture**: Each individual carries a genome of $L$ diallelic loci (states `0` or `1`).
* **Fitness Landscape**: Additive fitness across loci, where allele `0` confers a selective advantage of $0$ and allele `1` confers $s_i$ at locus $i$ ($W = \sum_{i=1}^L g_i s_i$).
* **Evolutionary Forces**: Genetic drift, natural selection, mutation, and linkage/recombination (introduced progressively across the notebooks).

---

## Repository Architecture

```text
.
├── notebooks/
│   ├── 01_genetic_drift.ipynb      # Core simulator & neutral genetic drift
│   ├── 02_selection.ipynb          # Single-locus selection & fixation probability
│   └── 03_advanced_topic.ipynb     # Multi-locus evolutionary extensions
├── requirements.txt                # Python package dependencies
└── README.md                       # Project documentation
