# Phishing URL Detection

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Directory Structure](#directory-structure)
- [Results](#results)
- [Conclusion](#conclusion)

---

## Introduction

The internet has become an integral part of modern life, offering immense convenience while also enabling malicious activities like phishing. Phishers use tactics like social engineering or creating fake websites to deceive individuals and organizations, aiming to steal sensitive information such as account credentials.

Machine Learning offers a powerful approach to combat phishing by identifying common patterns and characteristics of malicious activities. This project uses Machine Learning models to detect phishing URLs and classify them as safe or unsafe.

To explore the project, click [here](#).

---

## Installation

The code is written in  Python 3.13.1 If you don't have Python installed, download it [here](https://www.python.org/downloads/).

After cloning this repository, install the required libraries by running the following command in the project directory:
```bash
pip install -r requirements.txt
```

---

## Directory Structure

```
├── pickle
│   ├── model.pkl
├── static
│   ├── styles.css
├── templates
│   ├── index.html
├── Phishing.ipynb
├── Procfile
├── README.md
├── app.py
├── feature.py
├── phishing.csv
├── requirements.txt
```

## Results

### Model Performance

| Model                       | Accuracy | F1 Score | Recall | Precision |
|-----------------------------|----------|----------|--------|-----------|
| Gradient Boosting Classifier| 97.4%    | 97.7%    | 99.4%  | 98.6%     |
| Random Forest               | 96.7%    | 97.0%    | 99.3%  | 99.0%     |
| Multi-layer Perceptron      | 96.7%    | 97.0%    | 99.6%  | 98.2%     |
| Support Vector Machine      | 96.4%    | 96.8%    | 98.0%  | 96.5%     |
| K-Nearest Neighbors         | 96.0%    | 96.4%    | 98.6%  | 99.2%     |
| Decision Tree               | 95.8%    | 96.2%    | 99.1%  | 99.3%     |
| Logistic Regression         | 93.4%    | 94.1%    | 94.3%  | 92.7%     |
| Naive Bayes Classifier      | 60.5%    | 45.4%    | 29.2%  | 99.7%     |

### Feature Importance

The following features significantly contribute to phishing URL detection:
- `HTTPS`
- `AnchorURL`
- `WebsiteTraffic`
### OutPut
![Alt Text](![Screenshot 2025-01-05 225558](https://github.com/user-attachments/assets/97002560-521b-47ad-9cd9-12d792b1c20e)
)
![Alt Text](![Screenshot 2025-01-05 225957](https://github.com/user-attachments/assets/e6679c77-f8bc-4e77-aea1-0c7babe7a455)
)



---

## Conclusion

1. This project explores various machine learning models to detect phishing URLs and highlights the features most relevant to classification.
2. Building this project provided insights into feature engineering, hyperparameter tuning, and evaluating model performance.
3. Features like `HTTPS`, `AnchorURL`, and `WebsiteTraffic` play a crucial role in identifying phishing URLs.
4. Among the tested models, the **Gradient Boosting Classifier** achieved the highest accuracy of 97.4%, making it the most effective model for this task.

Feel free to explore and enhance the project!

