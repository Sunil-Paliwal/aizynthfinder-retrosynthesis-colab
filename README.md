# AiZynthFinder-Based Retrosynthesis Workflow

**Dr. Sunil Paliwal**  
Department of Chemistry and Chemical Biology  
Stevens Institute of Technology

---

This repository contains a Google Colab notebook designed to facilitate retrosynthetic planning using the AiZynthFinder architecture.
> **Note:** This repository and the associated notebook are currently in active development for educational purposes. The code is provided as-is, and feedback or suggestions for improvement from the community are welcomed.

## Overview

This work is based on the open-source software **AiZynthFinder**, as described in the paper: Genheden et al., *J. Cheminform* (2020) 12:70. The original software utilizes a Monte Carlo tree search and a neural network policy to recursively break down molecules into purchasable precursors.

**Paper link:** <https://doi.org/10.1186/s13321-020-00472-1>

---

### **Quick Start**

To get started with the retrosynthesis workflow, follow these three steps (steps 1 through 3) in order.

#### 1. Preparation

- First, ensure you are logged into your Google account.

- Open the notebook in Google Colab by clicking the link below. This opens the latest version directly from this GitHub repository:

    **[AiZynthFinder Notebook in Google Colab](https://colab.research.google.com/github/Sunil-Paliwal/aizynthfinder-retrosynthesis-colab/blob/main/AiZynthFinder_Retrosynthesis_Colab.ipynb)**

- Then, click **"Copy to Drive"** to save your own editable copy of the notebook.

#### 2. Setup & Run Cells

- **Cell #1**: Run this first by clicking the ▶ (play) button. It creates a separate Python 3.11 environment and installs `aizynthfinder` (pinned to version 4.4.1) and its dependencies into it.
- **Cell #2**: Run this second by clicking the ▶ (play) button to download the public USPTO models and ZINC stock collection.
- **Cell #3**: Run this last by clicking the ▶ (play) button to launch the interactive search interface.

#### 3. Perform Analysis

- Once the interface has appeared, you can enter a new SMILES string and click **"Run Search"** for each molecule. Results are shown below the button: search statistics followed by images of the top-ranked routes (up to 10).

  The search box comes pre-filled with Aspirin's SMILES (`CC(=O)Oc1ccccc1C(=O)O`) as an example, so you can click **"Run Search"** right away to see a working result before trying your own molecule.

> **Note:** The Python 3.11 environment and the downloaded models are stored in the temporary Colab session storage (`/content`), so they are lost when the session disconnects or is closed. After a disconnect, re-run all three cells (#1, #2 and #3) in order.

### Why does the notebook use a separate Python environment?

Colab's default Python version is now newer than the versions supported by AiZynthFinder (Python 3.10 to 3.12). On the default Colab Python, a plain `pip install aizynthfinder` fails with *"No matching distribution found for aizynthfinder"*. The notebook therefore installs AiZynthFinder into its own Python 3.11 environment (created with [`uv`](https://github.com/astral-sh/uv)) and runs each search there. The input box and the results are displayed in the notebook itself. This also makes the notebook resilient to future changes of Colab's default Python. The AiZynthFinder version is pinned to 4.4.1 (the latest release at the time of writing) so that results stay reproducible; to use a newer release, edit the version number in Cell #1.

---

### Attribution & Licensing

- **Article License:** The original article is licensed under a Creative Commons Attribution 4.0 International License.
- **Data Waiver:** The data from the original article is provided under the Creative Commons Public Domain Dedication waiver.
- **Software License:** The original AiZynthFinder software is distributed under the MIT License.

*Note: Modifications have been made to the original workflow to adapt it for the Google Colab environment.*

### References

Genheden, S., Thakkar, A., Chadimová, V. et al. AiZynthFinder: a fast, robust and flexible open-source software for retrosynthetic planning. J Cheminform 12, 70 (2020). <https://doi.org/10.1186/s13321-020-00472-1>
