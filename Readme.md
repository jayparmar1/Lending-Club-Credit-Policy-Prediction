
 # **📘 Lending Club Credit Policy Prediction (Deep Learning)**
   This project uses a **Deep Neural Network (DNN)** to predict whether a loan meets **Lending Club’s credit policy** (credit.policy = 1 or 0).\
   It includes **end-to-end steps**: loading data, preprocessing, encoding, scaling, training the model, evaluating it, and predicting on new loan applications.

 # **📦 Dataset**
   The dataset used is:
   1. ### **loan\_data.csv**
      This dataset contains:

- Borrower financial information
- Loan characteristics
- Purpose of loan
- Whether the loan meets credit policy (credit.policy)

⚠ **Dataset is NOT uploaded here due to size and licensing.**

 # **🔧 Preprocessing Settings**
   The following preprocessing steps were used throughout the project:
   1. ### **🔹 One-Hot Encoding**
      Applied to the categorical column:

- purpose → converted into 7 dummy variables\
  (purpose\_credit\_card, purpose\_debt\_consolidation, etc.)
 ### **🔹 Standard Scaling**
     Applied to all the numeric features:


     **🔹Train/Test Split**

     Train: 80%

     Test: 20%

     Validation Split: 20% inside training

     Batch Size: 32

     Epochs: 40

 # **🧠 Model Architecture**
   The model is built using **TensorFlow Keras Sequential API**.
    ### **Layers:**
- **Input Layer**
- **Dense(128, activation='relu')**
- **BatchNormalization()**
- **Dense(64, activation='relu')**
- **Dropout(0.3)**
- **Dense(32, activation='relu')**
- **Dense(1, activation='sigmoid')**
  1. ### **Model Summary**

     |**Property**|**Value**|
     | :- | :- |
     |**Model Type**|Deep Neural Network|
     |**Optimizer**|Adam|
     |**Loss Function**|Binary Crossentropy|
     |**Final Activation**|Sigmoid|
     |**Output**|Probability loan meets credit policy|
     |**Epochs**|40|
     |**Batch Size**|32|


# **📊 Model Performance**
   After training, the model achieved:
### **🔹 Validation Accuracy: ~95%**
### **🔹 Training Accuracy: ~97%**
### **🔹 Test Accuracy: ~95%**

      This means the model performs very well in predicting credit policy outcomes.

# **🛠 Technologies Used**
- **Python**
- **TensorFlow / Keras**
- **Scikit-Learn**
- **NumPy & Pandas**
- **Matplotlib / Seaborn**
- **Google Colab**
# **🙌 Thanks**


