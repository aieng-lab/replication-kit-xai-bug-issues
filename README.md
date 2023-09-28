# Replication Kit

This repository serves as the replication kit for the paper "Studying the explanations for the automated prediction of bug and non-bug issues using LIME and SHAP".

## Content

- `data/` contains our (intermediate) result data and `train_data_all.p`, obtained from the replication kit of [Herbold et al. (2020)](https://arxiv.org/abs/2003.05357)
- `plots/` contains the plot files created by the analysis (by `replication_notebook.ipynb`).
- `requirements.txt` contains the requirements to run the python code in the jupyter notebooks.
- `replication_notebook.ipynb` is the notebook containing the analysis of the data.
- `replication_notebook_rater_1.ipynb` is the notebook containing the analysis of the data specific to rater 1.
- `replication_notebook_rater_2.ipynb` is the notebook containing the analysis of the data specific to rater 2.
- `replication_notebook_rater_3.ipynb` is the notebook containing the analysis of the data specific to rater 3.

## Execution of the labeling process

The labeling process, including the fine-tuning of the model, was performed with the open source software [xai-toolbox](https://github.com/benjaminLedel/xai-toolbox). Installation steps and how to obtain the model for fine-tuning and prediction are documented there.

## Execution the analysis

For Ubuntu 20.04 the setup to start a Jupyter Lab for the execution of the notebooks can be:

```
sudo apt-get update
sudo apt-get install python3-venv build-essential python3-dev
git clone https://github.com/aieng-lab/replication-kit-xai-bug-issues
cd replication-kit-xai-bug-issues/
python3 -m venv venv
source venv/bin/activate
pip install jupyterlab
pip install -r requirements.txt
jupyter lab
```
