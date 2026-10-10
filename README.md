# Fake_News_detection_ML_project


**Project Description**

This project develops a machine-learning-based system to classify news articles as fake or real using textual data. It compares three supervised learning algorithms: Logistic Regression, Multinomial Naive Bayes and Random Forest. TF-IDF and CountVectorizer are used to convert text into numerical features and compare classification performance.

**Dataset Description**

The project requires two CSV files: train.csv and test.csv. Both files must contain the following columns:

- text: The news article's textual content.

- label: The article's class label, represented as 0 or 1.

The script assumes that 0 represents Fake and 1 represents Real. Verify this mapping against the original dataset documentation before interpreting results.

**Requirements**

Python 3

pandas

NumPy

scikit-learn

NLTK

Matplotlib

Seaborn

**How to Run the Project**

**Option 1: Google Colab (recommended)**

Open Google Colab and upload fake_news_detection.py.

Upload the dataset files train.csv and test.csv to the Colab session's Files section.

Ensure both CSV files are available at /content/train.txt and /content/test.csv.

Open a code cell and run:

%run /content/fake_news_detection.py

Wait for the script to complete data cleaning, text preprocessing, model training and evaluation.

**Option 2: Run locally**

Install the required libraries:

pip install pandas numpy scikit-learn nltk matplotlib seaborn

Place the Python script and both CSV files in the appropriate locations.

Update TRAIN_PATH, TEST_PATH and OUTPUT_DIR in the script to match your local file paths.

Run the script:

python fake_news_detection.py

**Output**

The script saves experiment results in the fake_news_results directory. Outputs include dataset audit summaries, class distributions, model performance metrics, confusion matrices, visualisations and a comparison of TF-IDF and CountVectorizer.

**Project Objective**

The objective is to evaluate traditional supervised machine learning algorithms for fake-news classification, identify the strongest-performing model and assess how text feature representation influences accuracy. Predictions indicate textual patterns learned from the dataset; they do not independently verify whether a news article is factually true.
