
# 🧠 K-Nearest Neighbors (K-NN) Classifier on Social Network Ads Dataset

This project implements a **K-Nearest Neighbors (K-NN)** classification model on a dataset containing **Age** and **Estimated Salary** features. The goal is to train the model to **predict the probability of whether a person will make a purchase or not** based on these features.

---

## 📁 Project Structure

- `Social_Network_Ads.csv`: Dataset file (must be uploaded in Colab runtime).
- Python script (in a Colab notebook) with the following steps:
  - Data preprocessing
  - Feature scaling
  - Model training (K-NN)
  - Predictions
  - Accuracy and confusion matrix evaluation
  - Decision boundary visualization for both training and test sets

---

## 🚀 How to Run in Google Colab

1. **Open this Notebook in Google Colab**  
   If you're not already in Colab, upload the notebook or open it from GitHub.

2. **Upload the Dataset**  
   Use the following cell to upload `Social_Network_Ads.csv`:
   ```python
   from google.colab import files
   uploaded = files.upload()
   ```

3. **Run Each Code Cell in Sequence**  
   The code will:
   - Preprocess the data
   - Train the model
   - Show prediction results
   - Visualize the decision boundaries for training and test sets

4. **Prediction Example**  
   The model predicts output for a new user with age 30 and estimated salary of $87,000.

---

## 📊 Dataset Details

- **Features**:
  - `Age`
  - `EstimatedSalary`
- **Target**:
  - `Purchased` (0: No, 1: Yes)

---

## 📈 Model Summary

- **Classifier**: `KNeighborsClassifier`
- **Parameters**:
  - `n_neighbors = 5`
  - `metric = 'minkowski'` with `p = 2` (Euclidean distance)
- **Evaluation**:
  - Confusion Matrix
  - Accuracy Score
- **Visualization**:
  - Colored decision boundaries for both training and test data

---

## 🤝 How to Contribute

We welcome contributions to improve this notebook or extend the model! Here's how you can help:

1. **Fork the repository** (if hosted on GitHub).
2. **Clone your fork**:
   ```bash
   git clone https://github.com/MaddyRizvi/K-Nearest-Neighbors-K-NN.git
   ```
3. **Create a new branch**:
   ```bash
   git checkout -b improve-feature-scaling
   ```
4. **Make your changes** (e.g., add cross-validation, improve visualizations).
5. **Commit your changes**:
   ```bash
   git commit -m "Enhanced data visualization and accuracy metrics"
   ```
6. **Push to your branch**:
   ```bash
   git push origin improve-feature-scaling
   ```
7. **Open a Pull Request** with a clear description of the improvement.

---

## 📌 Suggestions for Future Improvements

- Add cross-validation support
- Hyperparameter tuning for optimal `k`
- Interactive visualization using `plotly`
- Deploy with `Streamlit` for simple web interface

---

## 📧 Contact

For suggestions or queries, feel free to open an issue or contact the maintainer.


---

## 📄 License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2025 Syed Rizvi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

