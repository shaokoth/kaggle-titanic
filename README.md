# kaggle-titanic
This project predicts whether a passenger on the Titanic survived or not. It's a classic machine learning project based on the Kaggle competition.

## Feature Engineering
This project heavily relies on feature engineering to improve the model's performance. The following features were created:

- Title: Extracted from the passenger's name (e.g., Mr, Mrs, Miss, Master).
- FamilySize: The total number of family members on board (SibSp + Parch + 1).
- IsAlone: A boolean indicating if the passenger was traveling alone.
- AgeGroup: Age grouped into bins (Child, Teen, Young, Adult, Senior).
- FareBin: Fare grouped into quartiles.
- FarePerPerson: Fare per person in the family.
- Deck: The deck the passenger was on, extracted from the cabin number.
- Interaction Features:
    Age_Class: Interaction between Age and Pclass.
    Fare_Class: Interaction between Fare and Pclass.
    Sex_Class: Interaction between Sex and Pclass.
    IsWomanOrChild: A boolean indicating if the passenger is a woman or a child
## Setup

### Install Miniconda (if needed)
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

### Create environment
```bash
conda create -n venv python=3.12 -y
conda activate venv
pip install -r requirements.txt
```