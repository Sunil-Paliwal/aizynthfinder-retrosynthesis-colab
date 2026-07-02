# AiZynthFinder-Based Retrosynthesis Workflow
This repository contains a Google Colab notebook designed to facilitate retrosynthetic planning using the AiZynthFinder architecture.
> **Note:** This repository and the associated notebook are currently in active development for educational purposes. The code is provided as-is, and feedback or suggestions for improvement from the community are welcomed.
## Overview
This work is based on the open-source software AiZynthFinder, as described in the paper: Genheden et al., J. Cheminform (2020) 12:70. The original software utilizes a Monte Carlo tree search and a neural network policy to recursively break down molecules into purchasable precursors.
Paper link: https://doi.org/10.1186/s13321-020-00472-1
## Usage
•	**Open in Colab:** https://colab.research.google.com/drive/1y8034lT2tTQkdwb7bgVTxOHlFGiZmwF9?usp=sharing
•	**Setup:** Follow the instructions provided in the notebook cells to install the necessary environment, including rdkit, tensorflow, and networkx.

•	**Analysis:** Input your target molecule's SMILES string to perform retrosynthetic analysis using the included policy and stock configurations.
## Attribution & Licensing
•	**Article License:** The original article is licensed under a Creative Commons Attribution 4.0 International License.
•	**Data Waiver:** The data from the original article is provided under the Creative Commons Public Domain Dedication waiver.
•	**Software License:** The original AiZynthFinder software is distributed under the MIT License.
Note: Modifications have been made to the original workflow to adapt it for the Google Colab environment.
## References
Genheden, S., Thakkar, A., Chadimová, V. et al. AiZynthFinder: a fast, robust and flexible open-source software for retrosynthetic planning. J Cheminform 12, 70 (2020). https://doi.org/10.1186/s13321-020-00472-1
