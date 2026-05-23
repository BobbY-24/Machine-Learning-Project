# Machine Learning Classification Assignment

## Overview
I completed this repository as a machine learning assignment focused on supervised classification. I use a course-provided basketball performance dataset and evaluates classification accuracy across model settings.

## Motivation
This was early practice with model training, validation accuracy, and parameter comparison. I keep it documented as coursework context rather than presenting it as a flagship research project.

## Dataset
- **Source:** CognitiveClass / EDX machine learning course materials, based on notebook references.
- **File:** The notebook loads the dataset from the course environment.
- **Target variable:** The target is defined in the assignment notebook.
- **Known limitations:** Course datasets are designed for practice, so I do not draw broad real-world conclusions from this work.

## Methods
- I loaded a course-provided classification dataset.
- I trained and evaluated classification models.
- I compared validation accuracy across multiple K values for K-nearest neighbors.

## Results
My notebook reports validation accuracy of approximately **0.6667** across several tested K values.

## Key Insights
- This project helped me practice the basic supervised learning workflow.
- Validation accuracy stayed stable across the K values shown in the notebook output.
- The repo is useful as coursework history, while my newer projects show stronger documentation and framing.

## Limitations
- The dataset and assignment context are not fully self-contained.
- I include older course-environment assumptions.
- I treat this as a learning artifact, not a research project.

## How to Run
```bash
git clone https://github.com/BobbY-24/Machine-Learning-Project.git
cd Machine-Learning-Project
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook D-8-Assignment.ipynb
```
