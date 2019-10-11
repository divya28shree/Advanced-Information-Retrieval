# Advanced-Information-Retrieval
#  (CSE 586 - SUNY BUFFALO)
## Goal:
The goal of this project is to predict electoral violence in election prone countries.

## Data Collection and Filtering:
Three countries were taken into account *(India, Thailand and Indonesia)*. The project uses multiple datasource *(GDELT, Twitter, Acled)* to collect social unrest data for the past years. Only keywords related to elections are used to search the data to filter out the violence only related election. 

## Data Preprocessing and Feature Extraction:
*Google NLP* was used to extract features

## Word Embedding and Feature Selection:
For word embedding *GLOVE model* was used and to keep only relevant features *SVM-RFE(Recursive feature elimination)* was implemented.

## Prediction:
To predict the data, *Phased LSTM* was used as it provides with the implementation of multi-value data for each time step . Multi-time step prediction was implemented to predict for next n future dates.

## Evaluation:
Customized evaluation matrix was prepared to encorporate following factors:
a) Date
b) Location
c) Prediction Accuracy



