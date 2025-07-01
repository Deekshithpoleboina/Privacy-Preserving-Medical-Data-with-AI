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

### 📈 Model Used
- **GAN (Generative Adversarial Network)**
- Optional extensions with:
  - Variational Autoencoders (VAEs)
  - RNNs (for time-series data)

---

## 🔍 Features

| Feature      | Real Data (Standardized) | Synthetic Data (Sample Mean) |
|--------------|--------------------------|-------------------------------|
| Age          | 0.0 ± 1.0                | ~47.6                         |
| Cholesterol  | 0.0 ± 1.0                | ~298.2                        |
| Heart Rate   | 0.0 ± 1.0                | ~172.46                       |
| Sex          | 0.0 ± 1.0                | ~0.39                         |

*More features covered in full evaluation.*

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

👥 Team Members
P. Deekshith (2203A5170)

P. Sunil (2203A52169)

M. Prabhu Kumar (2203A52158)

D. Durga Prasad (2203A52146)

K. Tharun Chary (2203A52236)

🧑‍🏫 Guided By
Dr. Pramoda Patro, Associate Professor, School of CS&AI

🏫 Institution
SR University, Ananthasagar, Warangal, Telangana - 506371
Bachelor of Technology — School of Computer Science and Artificial Intelligence (2024–2025)

📚 References
Goodfellow et al. (2014). Generative Adversarial Nets. NeurIPS.

Esteban et al. (2017). Real-valued Medical Time Series Generation with GANs.

Ravuri & Reddy (2020). Privacy-Preserving Synthetic Data Generation: A Survey.

Chen et al. (2021). Synthetic Data in Machine Learning for Healthcare. Nature Biomedical Engineering.

📝 License
This project is for educational and research purposes. Please contact the authors for any reuse beyond academic exploration.

# Install dependencies
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn

# Run the notebook
jupyter notebook Ai_in_Healthcare_Project.ipynb
