# Genotype-phenotype maps using attention models

This repository contains the code and experimental data associated with the paper titled "Inferring genotype-phenotype maps using attention models" by Krishna Rijal et al.

## Repository structure

- `synthetic/`
  - `synthetic_data_attention_gaussian.ipynb`: Generates synthetic fitness data using Gaussian-distributed parameters and trains single-environment attention-based models for different values of $\epsilon$.
  - `synthetic_data_attention_exponential.ipynb`: Generates synthetic fitness data using exponentially distributed parameters. Trains single-environment attention-based models for different values of $\epsilon$.
  - `transfer_learning_synthetic_temps.ipynb`: Trains multi-environment attention-based models with varying amounts of data for a specific temperature. Evaluates their performance in a transfer learning setting.

- `experiment/`
  - `single_env_attention_QTL_yeast_data.ipynb`: Trains single-environment attention-based models for the 18 environments in the QTL budding yeast dataset. 
  - `multi_env_attention_QTL_yeast_data.ipynb`: Trains a multi-environment attention-based model for the 18 environments in the QTL budding yeast dataset.
  - `transfer_learning_QTL_yeast_temps.ipynb`: Investigates transfer learning by training multi-environment attention-based models with different amounts of data for a specific temperature in the QTL budding yeast dataset.

- `obtain_independent_loci.ipynb`: Identifies a set of loci where the SNP correlation between any two loci is below 94\%.

## Prerequisites

- Python 3.x
- Jupyter Notebook
- NumPy
- PyTorch
- Matplotlib
- SciPy
- GPUs (minimum Compute Capability 3.7 required by PyTorch)

##  **Usage**

Each Jupyter notebook in this repository is self-contained. The notebooks are organized into different directories based on their purpose. Appropriate functions are defined and described within the notebooks. The codes are well-commented to facilitate understanding and replication of the results.
