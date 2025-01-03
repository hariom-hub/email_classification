# email_classification
Classifying the email into spams or general messages using machine learning.

**Stages of the project**
*1. Data Cleaning
  2. EDA (Exploratory data analysis)
  3. Text Preprocessing
  4. Model building
  5. Improvement
  6. Website
  7. Deploy*

  *nltk.word_tokenize()* function is used to break the words from a sentence and then forms a list.
  *nltk.sent_tokenize()* function is used to break the number of words(sentences) from a sentence and then forms a list.
  *Naive Bayes algorithms applies well at the textual data*
  
  **Model Building**
  1. for model building we will firstly convert the textual data into numerical data by <b>Vectorization</b>
  2. Now we will use "Bag of Words" technique to create a column of most frequent words and then we will be checking those most frequent words with each messages.
  3. Word2vec is a machine learning technique that uses a shallow neural network to convert words into vectors that represent their meaning and relationships with other words.
  4. TF-IDF stands for term frequency-inverse document frequency, and it's a numerical statistic that measures the importance of words in a document. It's used in information retrieval and machine learning to: Quantify the relevance of words in a document, Help machine learning models read words, and Classify text.

***Naive Bayes - Gaussian Naive Bayes, Multinomial Naive Bayes, Bernoulli Naive Bayes.***

**Accuracy** and **Precision** are key metrics used to evaluate the performance of models, especially in classification, prediction, and measurement tasks. They have distinct meanings and applications:

---

### **Accuracy**  
- **Definition:** Accuracy measures how often the model correctly predicts the outcomes compared to the total number of predictions.
- **Formula:**  
  \[
  \text{Accuracy} = \frac{\text{Number of Correct Predictions}}{\text{Total Number of Predictions}}
  \]
- **Example:**  
  If a model correctly predicts 90 out of 100 cases, the accuracy is 90%.

- **Usage:** Accuracy is useful when all classes in the dataset are equally important and balanced.

- **Limitation:** In cases of **class imbalance** (e.g., one class is far more frequent than others), accuracy can be misleading. For instance, if 95% of the data belongs to one class, a model predicting only that class will still achieve 95% accuracy.

---

### **Precision**  
- **Definition:** Precision measures how many of the positive predictions made by the model are actually correct. It focuses on the quality of positive predictions.
- **Formula:**  
  \[
  \text{Precision} = \frac{\text{True Positives (TP)}}{\text{True Positives (TP)} + \text{False Positives (FP)}}
  \]

- **Example:**  
  If a model predicts 50 positive cases, but only 40 are correct, precision is \( \frac{40}{50} = 0.8 \) or 80%.

- **Usage:** Precision is crucial in applications where **false positives** are costly or undesirable (e.g., spam detection, fraud detection).

- **Limitation:** Precision does not consider false negatives, which can be important in some contexts.


### **Key Differences**
| Metric      | Focus Area                | Best for Cases Where           |
|-------------|---------------------------|---------------------------------|
| Accuracy    | Overall correctness       | Classes are balanced           |
| Precision   | Correctness of positives  | False positives are critical   |

Both metrics are often used alongside **recall** and **F1-score** for a more comprehensive evaluation of a model. Let me know if you'd like to explore these related metrics
     