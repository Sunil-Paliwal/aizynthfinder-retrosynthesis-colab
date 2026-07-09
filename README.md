# AiZynthFinder-Based Retrosynthesis Workflow
This repository contains a Google Colab notebook designed to facilitate retrosynthetic planning using the AiZynthFinder architecture.
> **Note:** This repository and the associated notebook are currently in active development for educational purposes. The code is provided as-is, and feedback or suggestions for improvement from the community are welcomed.

## Overview
This work is based on the open-source software **AiZynthFinder**, as described in the paper: Genheden et al., *J. Cheminform* (2020) 12:70. The original software utilizes a Monte Carlo tree search and a neural network policy to recursively break down molecules into purchasable precursors.

**Paper link:** [https://doi.org/10.1186/s13321-020-00472-1](https://doi.org/10.1186/s13321-020-00472-1)

### Quick Start

To get started with the retrosynthesis workflow, follow these steps in order. 

#### 1. Preparation
* First, click **"Sign in"** (top right) to log into your Google account.
* Open the notebook in Google Colab by clicking the link below:

  **[AiZynthFinder Notebook in Google Colab](https://colab.research.google.com/drive/1y8034lT2tTQkdwb7bgVTxOHlFGiZmwF9?usp=sharing)**
* Then, click **"Copy to Drive"** to save your own editable copy of the notebook.

#### 2. Setup & Run Cells
* **Cell #1**: Run this first by clicking the ▶ (play) button to install `aizynthfinder` and its dependencies.
* **Cell #2**: Run this second by clicking the ▶ (play) button to download the public USPTO models and ZINC stock collection.
* **Cell #3**: Run this last by clicking the ▶ (play) button to launch the interactive GUI.

#### 3. Perform Analysis
* Once the GUI has finished running, you can enter a new SMILES string into the interface and click **"Run Search"** for each molecule.

> **Note:** You only need to run all three steps when you start for the first time. If the Colab session disconnects or is closed, you generally only need to re-run Cell #2 and Cell #3 to restore the environment and GUI.

## Attribution & Licensing
* **Article License:** The original article is licensed under a Creative Commons Attribution 4.0 International License.
*	**Data Waiver:** The data from the original article is provided under the Creative Commons Public Domain Dedication waiver.
*	**Software License:** The original AiZynthFinder software is distributed under the MIT License.
  
*Note: Modifications have been made to the original workflow to adapt it for the Google Colab environment.*
## References
Genheden, S., Thakkar, A., Chadimová, V. et al. AiZynthFinder: a fast, robust and flexible open-source software for retrosynthetic planning. J Cheminform 12, 70 (2020). https://doi.org/10.1186/s13321-020-00472-1
