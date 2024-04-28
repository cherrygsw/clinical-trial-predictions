# HINT: Hierarchical Interaction Network for Clinical Trial Outcome Prediction


[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
[![GitHub Repo stars](https://img.shields.io/github/stars/futianfan/clinical-trial-outcome-prediction)](https://github.com/futianfan/clinical-trial-outcome-prediction/stargazers)
[![GitHub Repo stars](https://img.shields.io/github/forks/futianfan/clinical-trial-outcome-prediction)](https://github.com/futianfan/clinical-trial-outcome-prediction/network/members)



This repository serves as the host for HINT, a deep learning-based method designed specifically for predicting the outcomes of clinical trials. HINT utilizes advanced machine learning techniques to analyze and forecast the results of clinical studies, providing valuable insights into the effectiveness of treatments and interventions. This method is particularly useful for researchers and healthcare professionals looking to improve trial designs and predict therapeutic efficacies.
The repository can be mainly divided into three parts:
- [`benchmark`](https://github.com/futianfan/clinical-trial-outcome-prediction/tree/main/benchmark) which describes the process of curating benchmark dataset named **Trial Outcome Prediction (TOP)** which is used for clinical trial outcome prediction. 
- [`HINT`](https://github.com/futianfan/clinical-trial-outcome-prediction/tree/main/HINT) is the Hierarchical Interaction Network, a deep learning based method. 
- [`data`](https://github.com/futianfan/clinical-trial-outcome-prediction/tree/main/data) which stores processed data. 


The following figure illustrates the pipeline of HINT. 

<p align="center"><img src="./HINT/hint.png" alt="logo" width="810px" /></p>



## Table Of Contents 

- [Installation](#installation)
- [Benchmark Data](#benchmark) 
- [HINT: Learn and Inference](#hint) 
- [Tutorial (Jupyter Notebook)](#tutorial)
- [Contact](#contact) 

--- 

<a name="installation"></a>
## ⚙️ Installation

We build conda environment and uses `conda` or `pip` to install the required packages. See [`conda.yml`](https://github.com/futianfan/clinical-trial-outcome-prediction/blob/main/conda.yml) for all the packages. 

```bash
conda create -n predict_drug_clinical_trial python==3.7 
conda activate predict_drug_clinical_trial 
conda install -c rdkit rdkit  
pip install tqdm scikit-learn 
pip install torch
pip install seaborn 
pip install icd10-cm
```

We use following command to activate conda environment. 
```bash
conda activate predict_drug_clinical_trial
```

---


<a name="benchmark"></a>
## 📊 Benchmark Data

To standardize clinical trial outcome prediction, we have created a benchmark dataset named TOP (Trial Outcome Prediction), which incorporates extensive data components about clinical trials, including details on drugs, diseases, and protocols (eligibility criteria). All relevant scripts for accessing and manipulating this dataset can be found in [`benchmark`](https://github.com/futianfan/clinical-trial-outcome-prediction/tree/main/benchmark). 
Please see [`benchmark/README.md`](https://github.com/futianfan/clinical-trial-outcome-prediction/blob/main/benchmark/README.md) for details. 

---


<a name="hint"></a>
## 🤖 HINT: Learn and Inference 

After processing the data, we employ the Hierarchical Interaction Network (HINT) to tackle the following four tasks. The pipeline of HINT is depicted in the figure below. All the necessary scripts for implementing HINT can be found in the folder named [`HINT`](https://github.com/futianfan/clinical-trial-outcome-prediction/blob/main/HINT). 
Please see [`HINT/README.md`](https://github.com/futianfan/clinical-trial-outcome-prediction/blob/main/HINT/README.md) for details. 

### Prediction results

Added the prediction results in `./results` for all the three phases. 

### Trained model

The trained HINT models for all the three phases are available in `./save_model`.  

## 📚 Tutorial (jupyter notebook)


- `benchmark`: [`tutorial_benchmark.ipynb`](https://github.com/futianfan/clinical-trial-outcome-prediction/blob/main/benchmark/README.md) describes to us some key components of the data curation process. 
- `HINT`: [`tutorial_HINT.ipynb`](https://github.com/futianfan/clinical-trial-outcome-prediction/blob/main/HINT/README.md) shown to be a tutorial to learn and evaluate HINT step by step. 


<a name="contact"></a>
## 📞 Contact

Please contact cherrygsw@gmai.com for help or submit an issue.













