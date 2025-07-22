
# Employee Network Link Prediction 🔗📊

This project leverages **Logistic Regression** and **Random Forest Classifier** models to analyze a company’s internal email communication network. The goal is to **predict management roles, future employee connections, and estimate salaries** based on network graph data.

---

## 📁 Project Structure

```
employee-network-link-prediction/
│
├── data/
│   ├── Future_Connections.csv
│   ├── Future_Connections_testing.csv
│   ├── email_prediction_NEW.txt
│   └── true_node_salaries
│
├── graphs/
│   ├── A4_P1_G1 to A4_P1_G5
│   └── A4_graphs
│
├── images/
│   ├── Feature Importance Bar Chart.png
│   ├── Graph G with Top Predicted Edges.png
│   ├── Management Prediction Histogram.png
│   ├── Predicted Connection Probabilities Histogram.png
│   └── Sample of Future Connection Predictions.png
│
├── employee_network_link_prediction.py
├── .gitignore
├── LICENSE
└── README.md
```

---

## ✨ Features

- 📊 **Graph-based Analysis** using NetworkX
- 🔍 **Future Connection Prediction** using ML models
- 📈 **Visualization of Top Predicted Links**
- 🧠 **Feature Engineering** on graph metrics like clustering coefficient, degree, path length
- 🖼️ **Insightful Graph Visualizations** for edge predictions and management insights

---

---

## 📌 Algorithms Used

- **Logistic Regression**: For binary classification (management vs. non-management)
- **Random Forest Classifier**: For link prediction tasks
- **Graph Metrics**: Degree centrality, resource allocation index, Adamic-Adar index, preferential attachment, Jaccard coefficient, etc.

---

## ⚙️ How to Run

### 1. Install Requirements

```bash
pip install numpy pandas networkx scikit-learn matplotlib
```

### 2. Run the Notebook or Script

You can run the `employee_network_link_prediction.py` script (if converted to this repo) for:

- Data loading and preprocessing
- Graph statistics computation
- Training and evaluation of link prediction model

---

## 📊 Sample Results

### 🔹 Graph Statistics

```
G1 --> clustering: 0.0000, path_len: 6.53, std_deg: 3.30, max_deg: 54
G2 --> clustering: 0.4931, path_len: 43.80, std_deg: 0.16, max_deg: 5
G3 --> clustering: 0.4897, path_len: 39.01, std_deg: 0.16, max_deg: 5
G4 --> clustering: 0.0000, path_len: 8.16, std_deg: 2.91, max_deg: 39
G5 --> clustering: 0.3650, path_len: 8.53, std_deg: 0.64, max_deg: 7
```

### 🔹 Graph Classification (Based on Watts-Strogatz Characteristics)

```
['SW_H', 'SW_L', 'SW_L', 'SW_H', 'SW_H']
```

- `SW_H`: Small World High degree (low clustering, low path length, high max degree)
- `SW_L`: Small World Low degree (high clustering, high path length, low std deviation)

---

## 📌 Visuals

📌 **Feature Importance**
![Feature Importance](images/Feature%20Importance%20Bar%20Chart.png)

📌 **Top Predicted Links**
![Predicted Edges](images/Graph%20G%20with%20Top%20Predicted%20Edges.png)

📌 **Prediction Probability Histogram**
![Prediction Histogram](images/Predicted%20Connection%20Probabilities%20Histogram.png)

---

## 👨‍💻 Author

**Mukesh Thenraj**

---

## 📜 License

This project is open for educational and non-commercial use under the MIT license.
