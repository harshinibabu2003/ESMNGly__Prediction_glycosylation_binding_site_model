
# 🧬ESMNGly-N-Glycosylation Binding Site Prediction Model

**ESMNGly** is a deep learning-based tool that predicts **N-glycosylation binding sites** in proteins.  
Using **advanced sequence embeddings** from the **pretrained protein language model ESM-2** (Evolutionary Scale Modeling)  


---

## 🔍 How It Works

1. 📄 Takes a **protein sequence** as input
2. 🔬 Generates **ESM-2 embeddings** for the sequence
3. 🧠 Extracts **secondary structure features** from **NetSurfP-3.0**:
   - **Structural features**: `rsa`, `asa`, `q3`, `q8`
   - **Q3 probabilities**: `p[q3_H]`, `p[q3_E]`, `p[q3_C]`
   - **Q8 probabilities**: `p[q8_H]`, `p[q8_I]`, `p[q8_B]`, `p[q8_E]`, `p[q8_S]`, `p[q8_T]`, `p[q8_C]`
   - **Backbone torsion (dihedral) angles**: `phi`, `psi`
   - **Disorder prediction**: `disorder`
4. 🤖 Feeds combined embeddings + structural features into **trained models**
5. ✅ Predicts **potential N-glycosylation binding sites**

---

## 📦 Frameworks & Libraries

🧠 Embedding Extraction: ESM-2 (Hugging Face Transformers)

🔬 Secondary Structure Features: NetSurfP-3.0

📊 Model Training: TensorFlow / Keras

⚙️ Data Processing: NumPy, Pandas, Scikit-learn

📈 Visualization: Matplotlib, Seaborn

💻 Environment: Python 3.x

---
## 📊 Data Availability

The datasets used for training and evaluation are available on **google drive**

[![Google Drive](https://img.shields.io/badge/Google%20Drive-Access%20Dataset-green?logo=googledrive)](https://drive.google.com/drive/folders/1zdcsRDUCf2uLL62eeuqUYqpn1k95I6H5?usp=drive_link)  
---
## 📂 Sample Prediction  

Follow these steps to run a prediction:  

<img width="1910" height="964" alt="image" src="https://github.com/user-attachments/assets/55e7ca47-eaa8-49d8-8de1-34e7ac1cfd43" />


1️⃣ **Input a Protein Sequence** 

<img width="1919" height="965" alt="image" src="https://github.com/user-attachments/assets/2eff6de6-ddac-4cbc-b4a3-e501fea88a95" />


# ESMNGly-WEB TOOL

<img width="1901" height="1079" alt="image" src="https://github.com/user-attachments/assets/a02687c5-f56c-4aaf-84b7-9d0e776cd1d4" />

<img width="1881" height="1025" alt="image" src="https://github.com/user-attachments/assets/430a8107-1edc-47fe-bb33-839f5681ef22" />


<img width="1917" height="1079" alt="image" src="https://github.com/user-attachments/assets/4cd82c58-a3aa-4f50-b2ab-f9bd014fd178" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5e22352d-8230-4d1f-9439-3a4a78bde970" />


## Acknowledgements

Facebook AI Research for ESM-2,DTU Health Tech for NetSurfP-3.0,Hugging Face Transformers,TensorFlow / Keras / Scikit-learn,Open-source community 



