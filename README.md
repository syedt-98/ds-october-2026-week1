# Week 1 · Traditional Machine Learning

**Data Science & Agentic AI Programme** · Mon 5 Oct - Fri 9 Oct 2026

- **Main course repo:** <https://github.com/samuelts96/ds-october-2026> (programme syllabus and Git guide)
- **Training plan:** [syllabus/Week-1_Training_Plan.docx](syllabus/Week-1_Training_Plan.docx) (summarised below)
- **Progress tracking:** your *W1* card on the DS October Trello board
- **Daily scrum:** 09:15 every day
- **Tuesday 13 Oct presentation:** [PRESENTATION.md](PRESENTATION.md). Your dataset and problem statement are on your W1 Trello card

## Session materials

| Topic | Material |
|---|---|
| **Classification guide** (interactive HTML): binary classification, logistic regression, naive Bayes, SVM, decision trees, bagging & boosting algorithms, metrics (precision / recall / F1, why accuracy misleads, ROC-AUC), hyperparameters for each algorithm, cross-validation, overfitting vs underfitting | [materials/classification_guide.html](materials/classification_guide.html): download and open it in a browser |
| Imbalanced classification: 4 algorithms, overfitting vs underfitting, SMOTE vs undersampling, precision/recall/F1, ROC-AUC | [materials/imbalanced_classification.ipynb](materials/imbalanced_classification.ipynb) |

Setup for the notebook: `uv add pandas numpy matplotlib scikit-learn imbalanced-learn jupyter`

## How to work in this repo

1. **Fork** this repo on GitHub, then clone **your fork**.
2. Create a branch: `git checkout -b week1/<your-name>`
3. Each day, add your hands-on notebook (e.g. `day1_regression.ipynb`), then `git add .`, `git commit -m "message"` and `git push`.
4. On Friday, post the link to your branch as a comment on your Trello card and move the card to **Review**. You'll present your work on **Tuesday of Week 2**.

## Week at a glance

| Day | Date | Topics | Hands-on |
|---|---|---|---|
| 1 | Mon 5 Oct | ML fundamentals, regression, evaluation, bias-variance, regularisation | Linear → Multiple Linear → Ridge → Lasso |
| 2 | Tue 6 Oct | Classification, logistic regression, classification metrics, KNN, SVM | Logistic Regression → KNN → SVM |
| 3 | Wed 7 Oct | Decision Tree, Random Forest | Tree depth experiments; Decision Tree vs Random Forest |
| 4 | Thu 8 Oct | Gradient Boosting, XGBoost, K-Means clustering | Boosting vs Random Forest; K-Means with different K |
| 5 | Fri 9 Oct | Cross-validation, hyperparameter tuning, algorithm selection | End-to-end ML mini project + technical assessment |

---

## Day 1 · ML fundamentals, regression, bias-variance & regularisation

**1. Machine learning fundamentals**
- What is machine learning?
- Supervised vs unsupervised learning
- Regression vs classification
- Basic ML workflow
- Training vs test data

**2. Regression**
- What is a regression problem?
- Linear regression: simple vs multiple linear regression
- High-level intuition of how linear regression learns
- Practical implementation

**3. Regression evaluation**
- MAE, MSE, RMSE, R²
- Interpreting regression results

**4. Model generalisation**
- Bias and variance
- Underfitting and overfitting
- The bias-variance trade-off
- Training vs test performance
- How model complexity affects generalisation

**5. Regularisation**
- Why regularisation is needed
- Ridge regression: intuition, and how it helps control overfitting
- Lasso regression: intuition, and its feature-selection effect
- L1 vs L2 regularisation: a conceptual comparison

> **Hands-on:** implement and compare Linear Regression → Multiple Linear Regression → Ridge → Lasso. Evaluate with MAE, RMSE and R², and observe the impact of model complexity and regularisation.

## Day 2 · Classification, logistic regression, KNN & SVM

**1. Classification fundamentals**
- What is classification?
- Binary vs multi-class classification
- Classification workflow
- Prediction probability and threshold

**2. Logistic regression**
- High-level intuition
- The sigmoid function (conceptual)
- Classification threshold
- Practical implementation

**3. Classification evaluation**
- Confusion matrix: TP, TN, FP, FN
- Accuracy, precision, recall, F1 score
- ROC-AUC
- When to use precision vs recall

**4. K-Nearest Neighbours (KNN)**
- KNN intuition: similarity / distance-based prediction
- Choosing K
- The effect of scaling
- Strengths and limitations
- Practical implementation

**5. Support Vector Machine (SVM)**
- SVM intuition and the decision boundary
- Margin and support vectors (high level)
- Linear vs non-linear classification
- The kernel concept
- Important hyperparameters (conceptual)

> **Hands-on:** implement Logistic Regression → KNN → SVM. Evaluate and compare the models with appropriate classification metrics.

## Day 3 · Decision Tree & Random Forest

**1. Decision Tree**
- How a tree makes decisions: nodes, branches and leaves
- The splitting concept; Gini and entropy (high level)
- Tree depth and model complexity
- Overfitting in decision trees, and basic ways to control it

> **Hands-on:** build a decision tree, experiment with tree depth, evaluate the model, and observe underfitting vs overfitting.

**2. Random Forest**
- Why use multiple trees? Ensemble learning intuition
- Bagging (conceptual)
- Random feature selection
- Voting / aggregation
- How Random Forest reduces variance
- Important hyperparameters

> **Hands-on:** build a random forest, evaluate it, and compare it with a decision tree. Discuss performance, generalisation and interpretability.

## Day 4 · Boosting & unsupervised learning

**1. Gradient Boosting**
- Boosting intuition: sequential learning from previous errors
- Weak learners (high level)
- Learning rate, number of estimators and model complexity

**2. XGBoost**
- What XGBoost is and how it works (high level)
- Why it is popular for tabular data
- Important hyperparameters (conceptual)
- Practical implementation

> **Hands-on:** implement Gradient Boosting / XGBoost, evaluate it, and compare it with Random Forest.

**3. K-Means clustering**
- What is unsupervised learning? What is clustering?
- K-Means intuition: centroids and assigning points to clusters
- Choosing K: the elbow method and inertia
- Interpreting clusters

> **Hands-on:** implement K-Means, experiment with different values of K, and visualise and interpret the clusters.

## Day 5 · Validation, tuning & end-to-end ML

**1. Model validation**
- Why a train/test split alone may not be enough
- The validation concept
- Cross-validation and K-fold cross-validation
- Model generalisation

**2. Hyperparameter tuning**
- Parameters vs hyperparameters
- Why tuning is needed
- Grid search and random search
- Choosing an evaluation metric for tuning

**3. Algorithm comparison & selection**

How to choose an algorithm based on problem type, dataset characteristics, performance, interpretability, computational requirements, overfitting / generalisation, and business requirements.

**4. End-to-end ML mini project**

**5. Technical assessment**
- Algorithm-based questions
- Scenario-based questions
- Model selection questions
- Evaluation metric questions
- A short coding exercise
- Mini-project discussion

---

## Algorithm coverage

| Problem type | Algorithms |
|---|---|
| Regression | Linear Regression, Multiple Linear Regression, Ridge, Lasso, KNN |
| Classification | Logistic Regression, KNN, SVM, Decision Tree, Random Forest, Gradient Boosting, XGBoost |
| Unsupervised | K-Means |

## Setup

In your uv project:

```bash
uv add pandas numpy matplotlib scikit-learn xgboost jupyter
```
