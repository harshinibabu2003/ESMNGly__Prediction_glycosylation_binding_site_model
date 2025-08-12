
# 🧬 ESMNGly — N-Glycosylation Binding Site Prediction

**ESMNGly** is a deep learning-based tool that predicts **N-glycosylation binding sites** in proteins.  
Using **advanced sequence embeddings** from the **pretrained protein language model ESM-2** (Evolutionary Scale Modeling)  
and trained classification models, it helps researchers quickly identify potential glycosylation sites for further study.

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

## 📂 Project Structure

