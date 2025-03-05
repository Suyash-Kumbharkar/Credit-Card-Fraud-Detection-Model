
# Credit Card Fraud Detection Model

## 📌 Project Overview
This project implements a machine learning model to detect fraudulent credit card transactions using deep learning techniques. The goal is to accurately identify fraudulent transactions while minimizing false positives.

## 🚀 Features
- **Data Preprocessing**: Standardization and normalization for optimal training.
- **Neural Network Model**: Built using TensorFlow/Keras.
- **Performance Metrics**: Evaluation using Precision, Recall, F1-score, and AUC.
- **Visualization**: Plots for accuracy, loss, and AUC over epochs.
- **Classification Report**: Detailed evaluation with confusion matrix.

## 📁 Repository Structure
```
Credit-Card-Fraud-Detection-Model/
│── data/               # Folder for dataset (if applicable)
│── notebooks/          # Jupyter Notebooks for data analysis and model training
│── models/             # Saved trained models
│── src/                # Python scripts for modular implementation
│── results/            # Plots & reports generated from model training
│── README.md           # Project documentation
│── requirements.txt    # List of dependencies
│── .gitignore          # Ignore unnecessary files
```

## 🛠 Installation
Clone the repository and install the required dependencies:
```bash
git clone https://github.com/Suyash-Kumbharkar/Credit-Card-Fraud-Detection-Model.git
cd Credit-Card-Fraud-Detection-Model
pip install -r requirements.txt
```

## 📊 Dataset
The dataset used in this project is **creditcard.csv** from Kaggle, which contains:
- **Time**: The seconds elapsed between each transaction.
- **V1-V28**: Principal components obtained using PCA.
- **Amount**: Transaction amount.
- **Class**: Target variable (0 = Non-Fraudulent, 1 = Fraudulent).

## 🔍 Data Preprocessing
- **Standardization**: Scaling numeric features using `StandardScaler`.
- **Splitting**: 80% for training, 20% for validation.
- **Balancing**: Techniques to handle class imbalance (optional).

## 📌 Model Architecture
The model consists of:
- **Input Layer**: Matching feature count.
- **Hidden Layers**:
  - Dense (32 neurons, ReLU activation)
  - Dense (64 neurons, ReLU activation)
  - Dense (128 neurons, ReLU activation)
  - Dense (32 neurons, ReLU activation)
- **Output Layer**: Single neuron with Sigmoid activation.
- **Loss Function**: Binary Crossentropy.
- **Optimizer**: Adam.

## 🎯 Training and Evaluation
The model is trained for **100 epochs** using an **80-20 train-test split**. Performance is evaluated using:
- **Accuracy**
- **Precision & Recall**
- **F1-score**
- **AUC (Area Under Curve)**
- **Confusion Matrix**

## 📜 Results
After training, the classification performance is analyzed:
- **Precision**: Measures fraud detection accuracy.
- **Recall**: Measures model's ability to detect fraud.
- **F1-score**: Harmonic mean of precision and recall.
- **AUC-ROC Curve**: Helps in threshold selection.

## 📷 Visualizations
Training performance is visualized using:
- **Accuracy Plot**: ![Accuracy Graph](results/accuracy_plot.png)
- **Loss Plot**: ![Loss Graph](results/loss_plot.png)
- **AUC-ROC Curve**: ![AUC Graph](results/auc_plot.png)

## 🛠 How to Use
1. Place the dataset in the `data/` folder.
2. Run the Jupyter notebook in `notebooks/`.
3. Modify `src/` scripts to experiment with different models.
4. Visualize results in `results/`.

## 🤝 Contributing
We welcome contributions! Follow these steps:
1. **Fork** the repository.
2. **Create a branch** for your feature (`git checkout -b feature-branch`).
3. **Commit** your changes (`git commit -m 'Add new feature'`).
4. **Push** to GitHub (`git push origin feature-branch`).
5. **Submit a pull request**.

## 📃 License
This project is licensed under the **MIT License**. Feel free to use and modify it for your needs.

---

For any questions, contact [Suyash Kumbharkar](https://github.com/Suyash-Kumbharkar).

