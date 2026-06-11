# Parental Estrangement Network Analysis

This repository contains the code for the paper:
**"Mapping Estrangement: A Multi-Layer Network Analysis of Causal Attributions and Emotions in Reddit Narratives"**

## Overview

This project applies Natural Language Processing (NLP) and multi-layer network analysis to Reddit narratives from estranged adult children. Using the Attributional Theory of Motivation and Emotion (ATME; Weiner, 1985, 2014) as a theoretical framework, we map co-occurrence relationships between causal attributions and emotions.

## Data

Data were collected from two Reddit communities:
- r/EstrangedAdultChild
- r/EstrangedAdultKids

Posts were accessed via [Arctic Shift](https://arctic-shift.net), a publicly available Reddit data archive.

**Note:** Raw data is not included in this repository as Reddit user data cannot be publicly shared. To replicate this study, download the data from Arctic Shift and follow the preprocessing steps in `01_preprocessing.ipynb`.

## Pipeline

```
Raw JSONL (Arctic Shift)
    ↓
01_preprocessing.ipynb     — cleaning, deidentification
    ↓
02_labeling.ipynb          — causal attribution labeling (GPT-4o-mini)
    ↓
03_emotions.ipynb          — emotion labeling (GoEmotions) + user-level aggregation
    ↓
04_network_analysis.ipynb  — network construction, metrics, visualization
```

## Requirements

```
pip install -r requirements.txt
```

All notebooks are designed to run on Google Colab with Google Drive mounted.

## Citation

If you use this code, please cite:
> [Citation will be added upon publication]

## License

MIT
