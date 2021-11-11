# Classification - Random Forest & Deep Neural Network

This is a project for the Data Mining and Machine Learning course, [CEID](https://www.ceid.upatras.gr/en) University of Patras.

## Classification using Random Forest :evergreen_tree:

Our goal is to identify patients who are prone to stroke.

The [Stroke Prediction Dataset](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset) contains the following patient information:

- id: unique identifier
- gender: "Male", "Female" or "Other"
- age: age of the patient
- hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
- heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
- ever_married: "No" or "Yes"
- work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
- Residence_type: "Rural" or "Urban"
- avg_glucose_level: average glucose level in blood
- bmi: body mass index
- smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
- stroke: 1 if the patient had a stroke or 0 if not

What we did:
1. Dataset analysis and graphical visualization
1. Preprocessing - locate and handle missing values using the following methods:
    * column removal
    * fill in with the average of the column
    * fill in using Linear Regression
    * apply k-Nearest Neighbors ([kNN](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm))
1. After the preprocessing, a prediction is made whether a patient is prone or not to have a stroke using [Random Forest](https://en.wikipedia.org/wiki/Random_forest).
We split the dataset into training (75%) and test (25%) set and evaluate the performance of the model using f1 score, precision and recall metrics.

## Binary Classification using Random Forest :brain: - :zero: :one:

Our goal is to identify whether a given email is spam or not.

The [Spam or Not Spam Dataset](https://www.kaggle.com/ozlerhakan/spam-or-not-spam-dataset) contains two columns. The first
column consists of email texts while the second one indicates if it is spam or not: 1 for spam, 0 otherwise.
We convert text emails to vectors using a [matrix of TF-IDF features](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) to use them as an input to a neural network.
After training a 1-hidden layer dense neural network, a prediction is made whether an email is spam or not spam.
We split the dataset into training (75%) and test (25%) set and evaluate the performance of the model using f1 score, precision and recall metrics.

## Team 👪
[Agisilaos Kounelis](https://github.com/kounelisagis)\
[Ioannis Sina](https://github.com/IoannisSina)

