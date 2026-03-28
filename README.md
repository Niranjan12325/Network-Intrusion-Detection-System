#  Network Intrusion Detection System (IDS)

##  Overview

This project is a **Machine Learning-based Intrusion Detection System (IDS)** that classifies network traffic as **Normal** or **Attack**.
It uses supervised learning algorithms like **Decision Tree** and **Random Forest** to detect malicious activities based on network features.

---

##  Features

*  Detects cyber attacks from network traffic data
*  Uses Machine Learning models:

  * Decision Tree Classifier
  * Random Forest Classifier
*  Fast and lightweight implementation
*  Provides:

  * Accuracy score
  * Classification report (precision, recall, F1-score)
*  Encodes categorical features using Label Encoding
*  Applies feature scaling using StandardScaler

---

##  Technologies Used

* Python
* Pandas
* Scikit-learn

---

##  Dataset

The project uses a **sample network intrusion dataset (`sample_nids.csv`)**.

### Dataset Features:

* `duration` → Connection duration
* `protocol_type` → Protocol used (TCP/UDP)
* `service` → Network service (HTTP, FTP, etc.)
* `flag` → Connection status
* `src_bytes` → Data sent from source
* `dst_bytes` → Data received
* `label` → Target (normal / attack)

---

##  Installation & Setup

### Clone the repository

```bash
git clone https://github.com/your-username/ids-project.git
cd ids-project
```

### Install dependencies

```bash
pip install pandas scikit-learn
```

###  Run the project

```bash
python ids.py
```

---

##  How It Works

1. Load dataset using Pandas
2. Encode categorical features using LabelEncoder
3. Convert labels:

   * Normal → 0
   * Attack → 1
4. Split features and target
5. Apply StandardScaler for normalization
6. Train models:

   * Decision Tree
   * Random Forest
7. Evaluate models using:

   * Accuracy
   * Classification Report
8. Output prediction for each record

---

##  Sample Output

* Decision Tree Accuracy: ~90–100% (depends on dataset)
* Random Forest Accuracy: ~95–100%

Outputs:

* Normal / Attack prediction per record
* Precision, Recall, F1-score

---

##  Note

Currently, the same dataset is used for both training and testing, which may lead to **overfitting**.
For real-world applications, use proper train-test splitting.

---

##  Future Improvements

* Use real-world datasets like NSL-KDD
* Implement Deep Learning models
* Add real-time traffic monitoring
* Deploy using Django/Flask
* Visualize results using graphs

---

##  Use Cases

* Network security monitoring
* Cyber attack detection
* Educational ML projects
* Security research

---

##  Author

**Niranjan E**

---

##  Acknowledgement

This project is built for learning purposes and demonstrates the application of Machine Learning in cybersecurity.

---
