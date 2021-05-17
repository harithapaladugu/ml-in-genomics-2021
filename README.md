# 2021-ml-in-genomics

This repo contains the course material for the course *Feature selection in GWAS* given at the [Machine Learning in Genomics intensive week](https://data-psl.github.io/intensive-week-genomics/) (day 4).
The slides are from [Chloé-Agathe Azencott](https://cazencott.info/) and the practicals are adapted from https://github.com/chagaz/ds3-2018-genetics.

## Content of the course

This repo includes the slides of the lecture and the jupyter notebooks of the practical sessions.
The notebooks cover the same tools as the lecture:
- practical1:
	- T-test and Manhattan plots
	- Linear regression
	- Lasso
- practical2:
	- Elastic-net
	- Multi-task lasso
	- Network-constained lasso

The practicals require writting very little code: most questions are about commenting on the results.
Corrected version of the practicals are provided.

## Installation

- Clone the repository `git clone https://github.com/goepp/ml-in-genomics-2021/`

- You need to download the heavy files `athaliana_small.X.txt` and `athaliana_small.W.txt` [here](https://plmbox.math.cnrs.fr/d/7f1fd70570144d398322/) and place them in `practical/data/`.

### Quick setup from scratch

You need python3 and jupyter notebook. An easy way to set it up from scratch is:

- Download [https://conda.io/en/master/miniconda.html](miniconda).

- Create a conda environment: `conda create -n mlgen`.

- Activate the conda env: `conda activate mlgen`.

- Install Jupyter Notebook: `conda install -c conda-forge notebook`.

- Create your kernel: `python -m ipykernel install --user --name mlgen --display-name "Python (mlgen)"`

- Install modules:
```
conda install ipykernel seaborn pandas numpy scikit-learn matplotlib # modules used in the practical
```

### Getting started

Run the jupyter notebook from within the conda env:
```
conda activate mlgen
jupyter notebook
```
And your notebook should open in a web browser. Now select the kernel `Python (mlgen)` inside Jupyter Notebook.
You're good to go!
