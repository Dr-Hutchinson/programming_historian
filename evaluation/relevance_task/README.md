
# Dataset and Statistical Results

## Overview

This repository contains the dataset and statistical analysis results for the study on the agreement between GPT-4 and Mistral.

## Contents

- `complete_data.csv`: The complete dataset used for analysis.
- `statistical_results.csv`: Statistical summary of the analysis.
- `README.md`: This file.

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
| Relevance             | 0.9837  | 0.127              |
| Quote Extraction      | 0.9106  | 0.287              |
| Contextual Relevance  | 0.9187  | 0.274              |

## Usage

To load the dataset and statistical results, use the following code:

```python
import pandas as pd

# Load the dataset
data = pd.read_csv('complete_data.csv')

# Load the statistical results
results = pd.read_csv('statistical_results.csv')
```

## Contact

For any questions or issues, please contact [Your Name] at [your.email@example.com].
