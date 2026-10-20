# Machine Learning Classification Assignment

[![notebook](https://github.com/BobbY-24/Machine-Learning-Project/actions/workflows/notebook.yml/badge.svg)](https://github.com/BobbY-24/Machine-Learning-Project/actions/workflows/notebook.yml)

## Overview
This is a supervised-classification assignment from IBM's *Machine Learning with Python* course (ML0101EN, via edX). I use the course's college basketball dataset to predict how far a team goes in the postseason and compare classifier accuracy across model settings. The exercise prompts come from the course; the model code and results are mine.

## Motivation
This was early practice with model training, validation accuracy, and parameter comparison. I keep it documented as coursework context rather than presenting it as a flagship research project.

## Dataset
- **Source:** the course's copy of a college basketball dataset (`cbb.csv`, five seasons of Division I teams), downloaded from the course's public storage when the notebook runs.
- **Target variable:** `POSTSEASON`, the round where a team's season ended, for teams that reached the Sweet Sixteen or later.
- **Known limitations:** Course datasets are designed for practice, so I do not draw broad real-world conclusions from this work.

## Methods
- I filtered to Sweet Sixteen, Elite Eight and Final Four teams and standardized 21 features.
- I trained KNN, a decision tree, an SVM and logistic regression on 44 teams and validated on 12.
- I compared validation accuracy across K values for KNN, tree depths, and SVM kernels.

## Results
On the 12-team validation split, KNN reaches **0.667** accuracy for every K from 1 to 15, as do a depth-1 tree and a polynomial-kernel SVM; logistic regression (C = 0.01) reaches 0.583. With 12 validation teams, one prediction moves accuracy by 8 points, so these numbers do not separate the models.

## Key Insights
- This project helped me practice the basic supervised learning workflow.
- Validation accuracy stayed stable across the K values shown in the notebook output.
- The repo is useful as coursework history, while my newer projects show stronger documentation and framing.

## Limitations
- The data is downloaded from the course's storage, so the notebook needs network access.
- The validation split is tiny (12 teams), and the "test set" section scores the validation predictions.
- I treat this as a learning artifact, not a research project.

## How to Run
```bash
git clone https://github.com/BobbY-24/Machine-Learning-Project.git
cd Machine-Learning-Project
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook postseason_classification.ipynb
```

## License
MIT for my code and write-up (see `LICENSE`). The exercise prompts and the dataset belong to the IBM course and are not covered by it.
