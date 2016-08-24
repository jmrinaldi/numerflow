# numerflow
Data workflows for the numer.ai machine learning competition

## Status
I just started to work on this, and a lot is not optimal. I'm glad if you have
any feedback, so just open up an issue (if there isn't already one). If you
have specific tasks that you want to see implemented, hit me up via the issues,
twitter or slack (@rogue).

## Tasks
Currently implemented:
* fetch and extract the datasets

### Planned
* automated dataviz and analysis (seaborn, nbconvert executed) in a jupyter
notebook
* train and predict (WIP/not upstream yet)
* split and prepare training/prediction data

## Usage
Prepare the project:
```
pip install -r requirements.txt
```

To fetch the training data run
```
env PYTHONPATH='' luigi --local-scheduler --module tasks.numerai_fetch_training_data FetchTrainingData
```
