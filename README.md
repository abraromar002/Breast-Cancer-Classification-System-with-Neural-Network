#🧠 Breast Cancer Classification with Neural Networks
This project builds a Neural Network using TensorFlow/Keras to classify whether a tumor is benign (1) or malignant (0) based on various features in the breast cancer dataset.

📂 Dataset
Source: The dataset is loaded from a local file breast_cancer.csv

Samples: 569

Features: 30 numerical features

Target: label column (1 = Benign, 0 = Malignant)

🔧 Project Structure
نسخ
تحرير
├── breast_cancer.csv
├── breast_cancer_classifier.ipynb
├── README.md
📊 Data Preprocessing
Checked for missing values ✅

Normalized data using StandardScaler ✅

Features and labels split into X and y ✅

Train/test split: 80% train, 20% test ✅

🤖 Model Architecture
Built with Keras Sequential API:

Input Layer: 30 features

Hidden Layers: Dense layers with ReLU activation

Output Layer: 1 neuron with Sigmoid (binary classification)

Example:

python
نسخ
تحرير
model = Sequential([
    Input(shape=(30,)),
    Dense(16, activation='relu'),
    Dense(8, activation='relu'),
    Dense(1, activation='sigmoid')
])
🧪 Training
Loss Function: binary_crossentropy

Optimizer: adam

Metrics: accuracy

Trained for a suitable number of epochs with validation split.

📈 Evaluation
Evaluated on test set using:

Accuracy

Confusion Matrix

Visualization of training curves (loss & accuracy)

📦 Dependencies
bash
نسخ
تحرير
pip install pandas numpy scikit-learn matplotlib tensorflow
🚀 How to Run
bash
نسخ
تحرير
# Clone the repository or open the notebook
# Run the cells in Jupyter Notebook or Colab
