# FL-IDS-Intrusion-Detection
FL-IDS++: A Dynamic Federated Learning Framework for Intrusion Detection with Personalized Non-IID Data, Adversarial Resilience and Energy-Efficient Lightweight Models


# FL-IDS++: A Dynamic Federated Learning Framework for Intrusion Detection

FL-IDS++ is a privacy-preserving, energy-efficient Intrusion Detection System (IDS) built on **Federated Learning (FL)**. It addresses core challenges like **non-IID data**, **adversarial threats**, **communication overhead**, and **client heterogeneity** using a combination of:

- **FedProx** – Personalized regularization for heterogeneous data.
- **FedAvg** – Baseline aggregation mechanism.
- **FedDyn** – Dynamic client selection and adaptive weighting.
- **Federated Knowledge Distillation (FKD)** – Reduces communication by transmitting logits instead of full models.
- **Differential Privacy (DP)** – Protects against model inversion attacks.
- **FGSM-based Adversarial Training** – Improves robustness to evasion attacks.
- **Lightweight Models** – MLP, CNN, Bi-LSTM optimized for edge deployment.

---

## 📁 Project Structure

```bash
FL-IDS++
├── preprocessing.ipynb              # Data loading, cleaning, and Non-IID partitioning
├── fl_server.ipynb                  # FL server logic with FedAvg, FedProx, FedDyn
├── fl_client_MLP.ipynb              # MLP client training with DP, FKD, and adversarial defense
├── fl_client_BiLSTM.ipynb           # Bi-LSTM client version
├── fl_client_CNN.ipynb              # CNN client version
├── evaluation_metrics.ipynb         # Accuracy, Precision, Recall, F1-score, Confusion Matrix
├── attack_analysis.ipynb            # Adversarial test using FGSM injection
├── model_performance_visuals.ipynb  # Performance plots (ROC, Loss, Accuracy curves)
├── results_comparison.ipynb         # Model-wise and dataset-wise analysis
├── README.md
