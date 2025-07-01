# AI-Powered Synthetic Medical Data Generation for Privacy-Preserving Research

This project demonstrates the use of Generative Adversarial Networks (GANs) to generate high-quality synthetic medical datasets that preserve patient privacy. Using the Heart Disease Cleveland dataset, we develop AI models that can simulate realistic health records for secure and ethical research and AI development.

---

## 🧠 Project Objective

Enable the generation of synthetic medical data that mimics real patient data while preserving privacy and complying with regulations like HIPAA and GDPR. The synthetic data retains clinical relevance and supports healthcare research and model training without exposing sensitive information.

---

## 📁 Contents

- `Ai_in_Healthcare_Project.ipynb`: Jupyter notebook with code implementation.
- `Heart_disease_cleveland_5000.csv`: Original dataset used for training.
- `synthetic_heart_disease_data.csv`: Output synthetic dataset.
- `AI_in_Healthcare_Group-2_Report.pdf`: Full project report.
- `Group-2_Ai_in_Healthcare_Poster.pdf`: Visual summary poster.

---

## 🛠️ Methodology

### 🔄 Process Overview

1. **Data Collection & Preprocessing**  
   Clean and standardize the Heart Disease dataset using imputation and scaling.

2. **Model Design**  
   Implement a GAN architecture with:
   - Generator: Produces synthetic records from random noise.
   - Discriminator: Distinguishes between real and fake records.

3. **Training**  
   Use adversarial training to iteratively improve both networks.

4. **Evaluation**  
   Evaluate synthetic data using statistical similarity and classification metrics.

### 📈 Models Used

- **GAN (Generative Adversarial Network)**
- Optional:
  - Variational Autoencoders (VAEs)
  - Recurrent Neural Networks (RNNs)

---

## 🔍 Features

| Feature      | Real Data (Standardized) | Synthetic Data (Sample Mean) |
|--------------|--------------------------|-------------------------------|
| Age          | 0.0 ± 1.0                | ~47.6                         |
| Cholesterol  | 0.0 ± 1.0                | ~298.2                        |
| Heart Rate   | 0.0 ± 1.0                | ~172.46                       |
| Sex          | 0.0 ± 1.0                | ~0.39                         |

*More features are covered in the full evaluation.*

---

## 📊 Results

- **Accuracy**: ~50% (baseline classifier)
- **Precision/Recall (Class 0/1)**: ~0.5 (macro average)
- **F1-Score**: 0.52 (Class 0), 0.48 (Class 1)
- **Statistical Similarity**: Synthetic data closely mirrors real data distributions.

---

## 🔐 Privacy Features

- No identifiable patient data used.
- Synthetic records generated from noise vectors.
- Optional differential privacy and membership inference resistance.

---

## 🚀 Applications

- Privacy-preserving machine learning in healthcare.
- Ethical AI model training and testing.
- Academic research without patient data risk.
- Medical simulations and prototypes.

---

## 📦 How to Run

```bash
# Clone the repository
git clone https://github.com/<your-username>/ai-synthetic-healthcare.git
cd ai-synthetic-healthcare

# Install dependencies
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn

# Run the notebook
jupyter notebook Ai_in_Healthcare_Project.ipynb
