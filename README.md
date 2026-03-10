# DATA 620 – Project 1  

### Hospital Network Centrality Analysis

Author: Woodelyne Durosier  

Course: DATA 620 – Web Analytics  

Date: March 9, 2026  

---

## Project Overview

This project uses network analysis to examine the structural characteristics of hospitals in the United States. Hospitals are linked via shared Health Service Areas (HSA), which represent regional healthcare marketplaces.

The purpose is to use centrality measurements to determine whether different hospital types occupy distinct positions in the healthcare network.

---

## Dataset

The dataset comes from the Dartmouth Atlas of Health Care, which provides hospital-level structural information including:

- Hospital provider identifiers

- Health Service Area (HSA)

- Hospital type classification

- System affiliation

- Bed counts

Source:  

https://data.dartmouthatlas.org/supplemental/#hospital

---

## Network Structure

- Nodes: Hospitals  

- Edges: Hospitals located in the same Health Service Area (HSA)

Hospitals that share an HSA operate in overlapping healthcare markets and patient catchment areas.

---

## Centrality Measures

Two centrality measures were computed:

- Degree Centrality: Number of hospitals linked within the same HSA.

- Eigenvector Centrality: A hospital's impact based on its connections to other highly connected hospitals.

---

## Categorical Variable

Hospitals were grouped by Hospital Type:

- Acute Care Hospitals

- Critical Access Hospitals

- Integrated Academic Medical Centers

- Teaching Hospitals

- Long-Term / Non-Acute Hospitals

---

## Statistical Analysis

An ANOVA test was used to see if degree centrality differed between hospital types.

Results:

- F-statistic: 51.93  

- p-value: 6.25 × 10⁻⁴³

This demonstrates statistically significant differences in centrality between hospital groups.

---

## Key Findings

- Certain hospital types hold more central locations in the network.

- Integrated university medical centers and larger hospitals typically have better connections.

- Smaller hospitals, such as critical access institutions, are typically less central to regional healthcare networks.

---

## Tools Used

- Python

- Pandas

- NetworkX

- Seaborn

- Matplotlib

- SciPy

---

## Author

Woodelyne Durosier

