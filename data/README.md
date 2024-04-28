# data 

The processed data are derived from the ClinicalTrials.gov database as of February 20, 2021.

## data file 

- `data/raw_data.csv`: all the data samples in benchmark. 
- `data/phase_I_train.csv`: phase I training data. 
- `data/phase_I_valid.csv`: phase I validation data. 
- `data/phase_I_test.csv`: phase I test data. 
- `data/phase_II_train.csv`: phase II training data. 
- `data/phase_II_valid.csv`: phase II validation data. 
- `data/phase_II_test.csv`: phase II test data. 
- `data/phase_III_train.csv`: phase III training data. 
- `data/phase_III_valid.csv`: phase III validation data. 
- `data/phase_III_test.csv`: phase III test data. 
- `data/toy_train.csv`: training data used for toy model (tutorial). 
- `data/toy_valid.csv`: validation data used for toy model (tutorial). 
- `data/toy_test.csv`: test data used for toy model (tutorial). 
- `data/ADMET`: processed ADMET data. 
- `data/drugbank_mini.csv`: a demo of drugbank data
- `data/sentence2embedding.pkl`: a mapping from sentence in eligibility criteria to BERT embedding. 


## column of csv file

All the data files are provided in the CSV format and share a uniform header structure. We will show the meaning of the columns of csv file. 

- `nctid`: identifiers of a clinical trial
- `status`: the status of the clinical trial, it can be `completed`, `net yet recruiting`, `active`, `recruiting`, `suspended`, `terminated`, `unknown status`, `withdrawn`. 
- `why_stop`: the reasons why the trial stops. It can be empty. 
- `label`: binary outcome label, 0 means trial fails while 1 means success. 
- `phase`: the phase of the trial. phase I, or phase II, or phase III. 
- `diseases`: list of disease names. 
- `icdcodes`: list of icd-10 codes of diseases. 
- `drugs`: list of drug names. 
- `smiless`: list of SMILES of the drugs. 
- `criteria`: eligibility criteria. 


