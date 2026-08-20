# Gut-MetaTwin


## Introduction

We developed **Gut-MetaTwin**, a computational framework for systematically predicting human gut microbiome (HGM)-mediated drug metabolism. Gut-MetaTwin integrates retrosynthetic analysis with deep learning-based enzyme annotation to identify microbial drug metabolic reactions and quantify individualized microbiome drug-metabolizing capacity based on community composition and functional profiles.

Gut-MetaTwin establishes a quantitative link between HGM composition and drug metabolic function, enabling microbiome-informed prediction of personalized drug responses.

## Usage

- Download the Gut-MetaTwin package

       git clone https://github.com/LiLabTsinghua/HGMandDrug.git


- Create and activate environment

       conda create -n Gut_MT python=3.7
       conda activate Gut_MT


- Download required Python packages

       conda install ipykernel
       pip install biopython
       pip install fair-esm==2.0.0
       pip install gurobipy
       pip install matplotlib
       pip install numpy
       pip install pandas
       pip install plotly
       pip install pubchempy
       pip install rdchiral==1.1.0
       pip install rdkit-pypi==2022.9.5
       pip install rxnmapper==0.3.0
       pip install scikit-learn
       pip install seaborn
       pip install cobra
       pip install torch==1.13.1


## Reproducible Run

This project consists of three major modules, which should be executed in the following order. The **ECnumber_prediction** module should be executed first to annotate enzyme functions from microbial protein sequences. The **retrosynthesis** module then predicts potential drug metabolic reactions. The **analysis** module integrates predicted reactions, enzyme annotations, and microbiome profiles to quantify microbiome-mediated drug metabolic capacity.

The execution order is indicated in the filenames of the Jupyter notebooks within each module.

- **ECnumber_prediction:**  
  `./Code/ECnumber_prediction`

- **retrosynthesis:**  
  `./Code/retrosynthesis`

- **analysis:**  
  `./Code/analysis`


The data generated from the retrosynthesis and EC number prediction modules, including predicted metabolic reactions and enzyme functional annotations, are available on [`Zenodo`](10.5281/zenodo.xxxxx).


## Citation

None

## Contact

- Feiran Li ([@feiranl](https://github.com/feiranl)), Tsinghua Shenzhen International Graduate School, Tsinghua University, Shenzhen, China
- Ke Wu ([@wuke0714](https://github.com/wuke0714)), Tsinghua Shenzhen International Graduate School, Tsinghua University, Shenzhen, China


Last update: 2026-08-20