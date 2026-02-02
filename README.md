# 🚨 CIC-IoT2023 Intrusion Detection using Deep Learning

## 📌 Project Overview
This project focuses on detecting Distributed Denial of Service (DDoS) and other network attacks in **Internet of Things (IoT)** environments using deep learning techniques.  
Using the **CIC-IoT2023 dataset**, we analyze large-scale network flow data and build robust classification models to distinguish **benign** traffic from **malicious IoT attacks**.

The project evaluates and compares multiple deep learning architectures, including **Deep Neural Networks (DNN)**, **Convolutional Neural Networks (CNN)**, and a **Transformer-based model**, to study their effectiveness for IoT intrusion detection systems (NIDS).

---

## 📊 Dataset
- **Dataset:** CIC-IoT2023  
- **Source:** Canadian Institute for Cybersecurity (CIC)  
- **Type:** Network flow-based IoT traffic  
- **Traffic Categories:** Benign and multiple attack classes  
- **Features:** Flow-level statistical features (packet counts, durations, byte rates, protocol flags, etc.)

⚠️ Raw dataset files are not included in this repository due to size constraints.

---

## 🧠 Methodology
1. Data cleaning and preprocessing  
2. Removal of missing and infinite values  
3. Feature normalization and scaling  
4. Class restructuring to reduce misclassification  
5. Targeted class balancing for minority attacks  
6. Training and evaluation of deep learning models  

---

## 🛠️ Models Implemented
- **Transformer-based Model**  
  - Utilizes self-attention to capture long-range dependencies in network traffic features  
- **Deep Neural Network (DNN)**  
  - Fully connected architecture used as a strong baseline  
- **Convolutional Neural Network (CNN)**  
  - Adapted for tabular IoT traffic using 1D convolution  

---

## 📈 Evaluation Metrics
Model performance is evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  
- ROC-AUC  

---

## 📁 Project Structure
CIC-IoT2023/
│
├── notebooks/ # Jupyter notebooks for EDA and modeling
├── scripts/ # Data preprocessing and training scripts
├── results/ # Evaluation results and visualizations
├── README.md # Project documentation
└── requirements.txt # Python dependencies


---

## ⚙️ Technologies Used
- **Programming Language:** Python  
- **Frameworks & Libraries:** NumPy, Pandas, Scikit-learn, TensorFlow  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  
- **Version Control:** Git & GitHub  

---

## 🚀 How to Run
1. Clone the repository:
```bash
git clone git@github.com:realabdullahbinzubair/CIC-IoT2023.git
cd CIC-IoT2023

2. Install dependencies:
pip install -r requirements.txt

3. Run notebooks:
jupyter notebook

## 📌 Results & Findings
- Initial baseline models achieved approximately **85% accuracy** on the CIC-IoT2023 dataset  
- After architectural improvements, class restructuring, and targeted balancing, all deep learning models achieved **~99% accuracy**  
- The **Transformer, DNN, and CNN** models demonstrated strong generalization across multiple attack categories  
- Merging statistically similar attack types (**DoS and DDoS into a single Flood class**) significantly reduced misclassification  
- Results confirm the effectiveness of modern deep learning architectures for **IoT-based intrusion detection**  

---

## 🔮 Future Work
- Extend the Transformer architecture with additional attention layers  
- Perform fine-grained multi-class attack classification  
- Explore real-time IoT traffic ingestion and online inference  
- Optimize models for deployment on resource-constrained edge devices  
- Investigate explainable AI (XAI) techniques for security interpretability  

---

## 👤 Author
**Abdullah Bin Zubair**  
Computer Science | AI / ML & Data Science  

GitHub: https://github.com/realabdullahbinzubair  

---

## ⭐ Acknowledgements
- Canadian Institute for Cybersecurity (CIC)  
- CIC-IoT2023 Dataset contributors  










