# #7DaysOfCode Machine Learning Challenge

This project is part of the projects belonging to Alura's [7 Days of Code](https://7daysofcode.io/?utm_source=social&utm_medium=linkedin&utm_campaign=planejamentosocial&utm_content=7daysofcode-12/07#dados), a collection of practical challengs proposed to improve the skills in various fields. \
\
In this project, the goal is to create a machine learning model, using the [Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset), which can predict whether a song/track is popular or not.

## 1. Overview

This project is composed of the following parts:

- Data analysis
- Data processing
- Baseline model training and evaluation
- Data resampling
- Finding best model
- Training, evaluating, and saving best model found

## 2. Project Step-by-step

**Note:** The project was performed in a Kaggle notebook, so there may be a few differences depending on where to reproduce project. The Kaggle notebook can be accessed by [clicking here](https://www.kaggle.com/code/christophercamilo/7dayschallenge)

First of all, the file was loaded in the notebook. After that, the data was explored, checking the general dataset info, the distribution of values for each feature, the number of null values, and how was the popularity distribution. Then, the data was processed: null values and redundant data were removed, non-numerical features were converted to numerical values, a target column was created from the popularity feature, the data was scaled, and, finally, it was split in training and test sets. The training data was further split to get a validation portion to be used to evaluate the model.\
Once prepared the data, it was time to train a baseline model and evaluate its performance. Then, the data was resampled to deal with the class imbalance and, during an iterative process, the most performing model and resampling method from a list were selected. The selected model had its hyperparameters tuned to get the best model and it had its performance evaluated, this time also using a ROC-AUC curve graph. Finally, the selected model was tested on the test set, it was once again evaluated and saved as a pickle file.

## 3. Challenges

The most notable challenge in this project involved the hyperparameter tuning, mainly because it was a very time consuming step. In the Kaggle environment, it isn't possible to use GPU or TPU to accelerate model training, unless you're using it to train deep learning models. As a result, the hyperparameter tuning step itself tended to take about 80% of the required time to complete the project. \
Another challenge to be considered was the amount of steps required to fulfill the proposed requirements. It turned the project a bit longer, despite not necessarily meaning harder.

## 4. Conclusion and Next Steps

The final model has a great accuracy of near 100%, and preforms decently regarding precision. The class imbalance was the biggest obstacle regarding model's performance. As next steps, it is suggested to use the dataset to train deep learning models to check if they're more reliable while not being too much time consuming. 
