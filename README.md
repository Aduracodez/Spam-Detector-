# 📨 Spam Detector using Machine Learning

A simple yet effective **spam message classifier** built with Python and scikit-learn.
This project demonstrates how to preprocess text data, train a Naive Bayes model, and predict whether a given SMS message is **Spam** or **Ham** (not spam).

---

## 📖 Overview

This notebook walks through the full process of building a spam detection system using the **SMS Spam Collection dataset**. It covers:

* Data loading and cleaning
* Text vectorization with `CountVectorizer`
* Model training using `Multinomial Naive Bayes`
* Model evaluation (accuracy and classification report)
* Predicting on new text samples

---

## ⚙️ Features

✅ Clean and preprocess text messages
✅ Train/test split for unbiased evaluation
✅ Feature extraction using bag-of-words
✅ High-accuracy Naive Bayes classifier
✅ Easy to adapt to new datasets

---

## 🧩 Technologies Used

* **Python 3.8+**
* **pandas** — data manipulation
* **scikit-learn** — ML model, preprocessing, evaluation
* **Jupyter Notebook** — interactive development environment

---

## 📦 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/Spam-Detector.git
cd Spam-Detector
pip install -r requirements.txt
```

> Or manually install required packages:
>
> ```bash
> pip install pandas scikit-learn jupyter
> ```

---

## 🚀 Usage

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
2. Open `Spam_detector.ipynb`
3. Run all cells (`Kernel > Restart & Run All`)

The notebook will:

* Load the dataset from GitHub
* Train a model
* Display accuracy and performance metrics
* Predict whether a sample message is spam or not

---

## 🧠 Example

```python
sample_msg = ["Congratulations! You've won a free vacation. Reply now to claim!"]
sample_vec = vectorizer.transform(sample_msg)
prediction = model.predict(sample_vec)[0]
print("Prediction:", "SPAM" if prediction == 1 else "HAM")
```

**Output:**

```
Prediction: SPAM
```

---

## 📊 Results

| Metric    | Score |
| --------- | ----- |
| Accuracy  | ~98%  |
| Precision | 0.97  |
| Recall    | 0.96  |
| F1-score  | 0.96  |

*(Results may vary slightly depending on dataset split and preprocessing.)*

---

## 🧮 Model Workflow

1. **Load Data** → Read dataset and assign labels
2. **Preprocess** → Clean and tokenize text
3. **Vectorize** → Convert to numerical form using bag-of-words
4. **Train Model** → Fit `MultinomialNB` on training data
5. **Evaluate** → Measure performance on test set
6. **Predict** → Classify new unseen messages

---

## 📈 Future Improvements

* Switch to **TF-IDF vectorization**
* Add **n-grams** for better context understanding
* Implement a **Streamlit web app** for live predictions
* Experiment with **Logistic Regression** or **SVM**

---

## 📜 License

This project is open-source under the **MIT License**.
Feel free to use and modify it for learning or your own projects.

---

## 🙌 Acknowledgements

* [SMS Spam Collection Dataset (UCI Machine Learning Repository)](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)
* [Data School’s PyCon Tutorial](https://github.com/justmarkham/pycon-2016-tutorial) for the dataset and inspiration.

---

⭐ If you found this project helpful, please give it a star on GitHub!
