# Dataset and Statistical Results

## Overview

This repository contains the dataset and statistical analysis results for the study on the agreement between GPT-4 and Mistral on a relevance determination task in a retrieval augmented generation (RAG) pipeline.

## Contents

- `complete_data_unscored.csv`: The original dataset used for analysis.
- `complete_data_scored.csv`: The dataset scored by GPT-4 for analysis of a relevance determination task by Mistral.
- `statistical_results.csv`: Statistical summary of the analysis.
- `README.md`: This file.
- `Evaluation_Notebook.ipynb`: Juypter Notebook containing code used to run this analysis.

## Data Description

### complete_data.csv

| Column                | Description                           |
|-----------------------|---------------------------------------|
| Scored_Relevance      | Relevance score (1 or 0)              |
| Scored_Extraction     | Quote extraction score (1 or 0)       |
| Scored_Context        | Contextual relevance score (1 or 0)   |
| ...                   | ...                                   |

### statistical_results.csv

| Metric                | Mean    | Standard Deviation |
|-----------------------|---------|--------------------|
| Relevance             | 0.9594  | 0.1983             |
| Quote Extraction      | 0.8211  | 0.3848             |
| Contextual Relevance  | 0.7561  | 0.4312             |

## Usage

To load the dataset and statistical results, use the following code:

```python
import pandas as pd

# Load the dataset
data = pd.read_csv('complete_data_unscored.csv')

# Load the statistical results
results = pd.read_csv('statistical_results.csv')
