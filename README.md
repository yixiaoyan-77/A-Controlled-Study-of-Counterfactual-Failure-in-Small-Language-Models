# A Controlled Study of Counterfactual Failure in Small Language Models

This repository contains the code and materials for the project **"A Controlled Study of Counterfactual Failure in Small Language Models: Lexical Bias or Reasoning Deficit?"**

We investigate whether small pre-trained language models (DistilBERT, BERT-base) fail at counterfactual detection due to **lexical surface bias** or a **genuine lack of causal reasoning**. The study combines **lexical perturbation** and **cross-distribution linear probing** on the SemEval-2020 Task 5 dataset.

## Repository Contents
.
├── README.md
├── requirements.txt
├── dsai5207.ipynb # Main notebook – reproduces all experiments
├── data/
│ └── README.md # How to obtain the dataset
├── figures/ # Output figures from the experiments

## Getting Started

### 1. Environment Setup

Install the required packages (preferably in a virtual environment or Google Colab with GPU runtime):

```bash
pip install -r requirements.txt

### 2. Obtain the Dataset
The dataset is SemEval-2020 Task 5 Subtask 1 (Counterfactual Detection).
Due to licensing, the dataset files are not included in this repository.
Please follow the instructions in data/README.md to download the two required CSV files (subtask1_train.csv and subtask1_test.csv) and place them in the data/ folder.

### 3. Run the Experiments
The entire pipeline is contained in a single Colab notebook: dsai5207.ipynb.
Open it in Google Colab (or Jupyter), make sure the runtime type is set to GPU, and run all cells in order.

The notebook will:

Load the dataset from data/

Fine-tune DistilBERT and BERT-base on counterfactual detection

Perform lexical perturbation evaluation

Run full-set and generalisation linear probes on hidden representations

Generate figures (saved to figures/)
