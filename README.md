# Invasive Species Monitoring
## Identify images of invasive hydrangea
### Kaggle Competition 

**Athors :** Cédric FLAMANT & Axel CHENU 
**Creation date :** 08/01/2020
**Update date :** 14/01/2021


## Data Description 
This data is taken from kaggle, the `data` folder contains original data from kaggle.

- **train.7z** = the training set (contains 2295 images).
- **train_labels.csv** = the correct labels for the training set.
- **test.7z** = the testing set (contains 1531 images), ready to be labeled by your algorithm.
- **sample_submission.csv** = a sample submission file in the correct format.

### Data fields
- **name** = name of the sample picture file (numbers)
- **invasive** = probability of the picture containing an invasive species. A probability of 1 means the species is present.

Kaggle : https://www.kaggle.com/c/invasive-species-monitoring/overview

## PROJECT DEVELOPMENT
### Model builder

* [`model_builder/`](model_builder/) contains scripts for building the scikit-learn model used by the app:

* [`02.Split_data.ipynb`](model_builder/02.Split_data.ipynb)
* [`03.Featurize_data.ipynb`](model_builder/03.Featurize_data.ipynb) (which reuses [`featurizer.py`](src/featurizer.py) from the `src/` directory)
* [`04.Train-model.ipynb`](model_builder/04.Train-model.ipynb)
* [`05.Prediction.ipynb`](model_builder/05.Prediction.ipynb)

### Notebooks 
01. GET DATA
The `data` folder contains original data from kaggle
Direct connection by using Kaggle CLI

02. SPLIT DATA
Separation of data into training data and validation data (75/25)

03. FEATURIZE
Removal of categorical fields: url and boilerplate columns

04. TRAIN MODEL 
* 
* 

Model storage: `model.pkl`

05. PREDICTION 
* Prediction using the save model
* Save the submission: `data / submission.csv`
* By Kaggle CLI we submit our results

## SCORES 
FIRST TEST on 14/01/2021
* Score of 
* suppression des features text
* Pre processing automatic by deepnote 

SECOND TEST on 08/01/2021
* Score of ** **
* a
* a


## Requirements
* [`requirements.txt`](requirements.txt) lists the requirements for running the app "in production", on the Algorithmia platform. It can be generated from the Python environment you used to build the model by running [`requirements.py`](requirements.py).
* [`requirements-dev.txt`](requirements-dev.txt) is where you would customize the list of requirements for this project. It is used by DeepNote upon starting up the project, for initializing the environment.

## Copyright
[Cédric FLAMANT](https://github.com/Drice33)
[Axel CHENU](https://github.com/ACHENU26)