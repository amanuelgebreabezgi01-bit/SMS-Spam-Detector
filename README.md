# SMS Spam Detector

## Project Overview
This project uses Machine Learning and Natural Language Processing (NLP) to classify SMS messages as either **Spam** or **Ham (Legitimate)**.

The model uses TF-IDF for text feature extraction and Multinomial Naive Bayes for classification.

## Objectives
- Build an SMS spam detection model.
- Convert text messages into numerical features using TF-IDF.
- Train a Multinomial Naive Bayes classifier.
- Evaluate the model using test data.
- Test the model with custom messages, including challenging examples.

## Dataset
The project uses the **UCI SMS Spam Collection Dataset**.

Dataset link: https://archive.ics.uci.edu/dataset/228/sms+spam+collection

The dataset contains 5,574 SMS messages labeled as spam or ham.

The dataset is downloaded and loaded in Google Colab. It is not included in this GitHub repository.

## Technologies Used
- Python
- Google Colab
- Pandas
- Scikit-learn
- TF-IDF Vectorizer
- Multinomial Naive Bayes
- GitHub

## Methodology
1. Download and load the SMS dataset.
2. Explore and inspect the dataset.
3. Convert labels into numerical values.
4. Split the data into training and testing sets.
5. Convert text messages into TF-IDF features.
6. Train a Multinomial Naive Bayes classifier.
7. Evaluate the model using test data.
8. Test the model using custom messages.

## Model Performance

| Metric | Result |
|---|---:|
| Accuracy | 96.05% |
| Testing messages | 1,115 |
| Correct predictions | 1,071 |
| Incorrect predictions | 44 |

## Custom Message Testing

The model was also tested using eight custom messages.

- Correct predictions: 7
- Incorrect predictions: 1
- Custom test accuracy: 87.5%

One challenging spam message, containing deliberately altered words such as `Cl@im`, `fr33`, and `g1ft`, was incorrectly classified as Ham.

This demonstrates that unusual spelling can make spam detection more difficult.

## Challenges and Lessons Learned
- Unusual spelling can reduce classification accuracy.
- Words can have different meanings depending on context.
- A high accuracy score does not mean a model is perfect.
- Testing with custom examples helps identify model weaknesses.

## What I Learned
I learned how to preprocess text messages, extract numerical features using TF-IDF, and train a Multinomial Naive Bayes classifier.

I also learned how to evaluate a machine learning model, test its limitations, and manage a project using GitHub branches, commits, and pull requests.

## Repository Structure

```text
SMS-Spam-Detector/
│
├── spam_filter.ipynb
└── README.md
```

## How to Run
1. Open `spam_filter.ipynb` using Google Colab.
2. Run the notebook cells from top to bottom.
3. The notebook downloads the dataset automatically.
4. Follow the evaluation and custom testing sections.

## Author
Machine Learning Project – SMS Spam Detection
