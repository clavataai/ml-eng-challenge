# **Take-Home Challenge: Text Classification Pipeline**

## **Objective**

Your task is to create a machine learning pipeline to classify online user comments as either **"safe"** or **"unsafe"**. The goal is to accurately identify potentially harmful or offensive comments, making this a practical challenge in text classification for content moderation.

This project is designed to evaluate your skills in data processing, feature engineering, model development, and engineering practices to structure a reliable ML pipeline.

---

## **Dataset**

We’ll be using the **[Wikipedia Talk Labels: Personal Attacks](https://www.kaggle.com/datasets/jigsaw-team/wikipedia-talk-labels-personal-attacks/data)** dataset, which includes comments from Wikipedia talk pages with labels indicating different forms of attacks.

1. **Classes**:

   - **Unsafe**: Aggregate comments labeled with any of the "attack" attributs into a single "unsafe" class. (i.e., "quoting_attack" and "recipient_attack" all become just "unsafe").
   - **Safe**: All other comments can be grouped into a "safe" class.

2. **Data Preparation**:
   - **Training Data**: Use the provided labeled dataset to train your model.
   - **Evaluation Data**: Hold out a portion of the data for final evaluation to simulate a real-world test set. (Avoid manually inspecting or optimizing on the held-out data to maintain its integrity.)

---

## **Requirements**

### 1. **Data Processing and Feature Engineering**

- **Preprocessing**: Write functions or modules to preprocess the comments, handling text cleaning, tokenization, and any necessary normalization steps.
- **Feature Engineering**: Generate features suitable for text classification, such as word embeddings (e.g., TF-IDF, Word2Vec, or BERT embeddings). Explain any decisions made for feature selection.

### 2. **Model Training and Selection**

- **Model Choice**: Train a classification model that can distinguish between "safe" and "unsafe" comments. You are free to choose any machine learning or deep learning model but should justify your selection based on accuracy, interpretability, and computational efficiency.
- **Comparative Analysis**: If possible, compare a few different model architectures (e.g., traditional ML models vs. neural networks) and report which one performs best and why.

### 3. **Model Evaluation**

- **Metrics**: Use evaluation metrics that are relevant for imbalanced data, such as precision, recall, F1-score, and ROC-AUC.
- **Analysis**: Provide insights into model performance, including any limitations or areas for improvement. Use plots, if appropriate, to visualize model effectiveness.

### 4. **Pipeline Structure**

- **Code Structure**: Develop the solution as an end-to-end pipeline, ideally executable with a single command/script or a structured notebook. Ensure that the pipeline is modular, with clear, reusable functions for each stage (preprocessing, feature extraction, training, evaluation).
- **Scalability Considerations**: Consider how your code could handle unseen data and be adapted to larger datasets.

### 5. **Documentation**

- **README**: Include a README file with clear instructions for running your code, any dependencies, and an overview of your approach.
- **Explanations**: Add comments or a short report explaining design decisions, model choice, and potential future improvements.

---

## **Deliverables**

1. **Code**: A well-structured codebase or notebook that implements your pipeline.
2. **Model and Performance Summary**: Include your selected model and a summary of its performance on the held-out test set.
3. **Documentation**: A README file with setup instructions and your approach overview, along with comments in your code or a brief report discussing your solution.

---

## **Evaluation Criteria**

1. **Technical Completeness**:

   - Does the solution cover all core steps, from data processing to evaluation?

2. **Code Quality and Modularity**:

   - Is the code modular, clean, and ready for production? Does it follow best practices and handle real-world data challenges effectively?

3. **Modeling Choices**:

   - Is there a sound rationale behind model selection, and does the model perform effectively based on the metrics provided?

4. **Documentation and Communication**:

   - Are instructions clear and concise? Has the candidate effectively communicated the solution and insights?

5. **Deployment Readiness** (Optional Bonus):
   - Extra credit for candidates who package the pipeline in a deployable format (e.g., Docker, API endpoint).

---

## **Submission Instructions**

- **Deadline**: Submit your solution within 7 days of receiving the challenge.
- **Format**: Compress your code, model, and documentation in a `.zip` file or provide a link to a GitHub repository.
- **Contact**: If you encounter any issues, feel free to reach out to us!

---

Good luck, and we look forward to reviewing your submission!

> Note: If for some reason you are unable to obtain the datasets from Kaggle, we can provide them as a `zip` file.
