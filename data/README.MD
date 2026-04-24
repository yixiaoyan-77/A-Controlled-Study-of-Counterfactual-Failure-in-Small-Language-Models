# Dataset: SemEval-2020 Task 5 Subtask 1

This directory should contain the following two files:

- `subtask1_train.csv`
- `subtask1_test.csv`

## Obtaining the Data

The official SemEval-2020 Task 5 dataset is available on Zenodo:

1. Visit the **SemEval-2020 Task 5** Zenodo page:  
   [https://zenodo.org/record/3932363](https://zenodo.org/record/3932363) (or search for “SemEval-2020 Task 5” on Zenodo)

2. Download the files:
   - `subtask1_train.csv`
   - `subtask1_test.csv`

3. Place both files into this `data/` folder.

## Data Format

Each file is a comma-separated CSV with the following columns:

- `sentenceID`: unique identifier
- `gold_label`: 1 for counterfactual, 0 for not counterfactual
- `sentence`: the text of the sentence

The training set contains approximately 13,000 sentences; the test set contains 7,000. The labels are highly imbalanced (~11% counterfactual).

## Usage in the Notebook

If you store them elsewhere, adjust the file paths in the notebook accordingly.                                                                          
