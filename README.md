# GR-EN-A-DE-A-Novel-Graph-Based-Model-for-online-Extremist-Narrative-Analysis

Repository of the paper: GR-EN-A-DE: Graph Modelling of Extremist Narrative Analysis


## Datasets

Below are the main datasets used in this project, with both their description and the corresponding **class names** to use in the code (see `preprocessing.py`):




---
## Losses

## 1. Contrastive Loss 

**Purpose:**  
To make sure the representation (embedding) of the same node under two different graph views is very similar, and the representations of different nodes are clearly distinct.

**How does it work, step by step?**

1. **For each node,** we create two "views" (versions with small random changes).
2. **We measure similarity** between the same node under different views using cosine similarity, which tells us how close or aligned two vectors are (1 means identical, -1 means opposite).
3. **We want this similarity to be as high as possible for the same node.**
4. **But for other nodes,** we want the similarity to be low.
