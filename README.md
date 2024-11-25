Fake News Detection Project
This project is aimed at detecting fake news using a machine learning model trained on a dataset containing both fake and true news articles. It utilizes natural language processing (NLP) techniques, such as TF-IDF vectorization, to preprocess and transform the data before training a logistic regression model for classification.

Features
Data Preprocessing:

Merges true and fake news datasets.
Cleans text data by removing unwanted characters such as URLs, digits, and special characters.
Machine Learning Model:

A logistic regression classifier trained to differentiate between fake and genuine news.
Prediction System:

After training, the model can predict whether a given news article is genuine or fake.
Libraries Used
pandas: For data manipulation and analysis.
re: For regular expression-based text cleaning.
sklearn: For implementing machine learning algorithms and text vectorization.
pickle: For saving and loading models (if needed).
Installation
To run the Fake News Detection project, make sure you have the necessary libraries installed. You can install them using pip:

bash
Copy code
pip install pandas scikit-learn
How to Run
Clone or download the project files to your local machine.
Place your true.csv and fake.csv datasets in the appropriate directory (Fake_News_Detection/data/).
Run the Python script:
bash
Copy code
python model.py
You will be prompted to input news text. Enter the news article to check if it's fake or genuine.
Example Usage
bash
Copy code
Do you wanna check the genuinity of some news? Y/N? y
Paste the news to be checked below:

"New study reveals the benefits of drinking water for your health."
The system will then output:
GENUINE NEWS if the news is true.
FAKE NEWS if the news is identified as fake.
Model Evaluation
After training the model, the accuracy and classification report are displayed for evaluation. The model's score will show how well it performs on the test data.

Example output:

markdown
Copy code
The score of your model is 0.94

BELOW IS THE CLASSIFICATION REPORT ON THE MODEL;
              precision    recall  f1-score   support

           0       0.95      0.96      0.95       100
           1       0.93      0.92      0.93        80

    accuracy                           0.94       180
   macro avg       0.94      0.94      0.94       180
weighted avg       0.94      0.94      0.94       180
Notes
The model currently uses Logistic Regression for classification.
The text is cleaned using a custom function (wordopt) that removes URLs, digits, and other irrelevant characters.
