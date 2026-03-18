# 📌 PCA vs t-SNE on MNIST & Face Dataset

## 🚀 Project Overview
This project explores and compares **dimensionality reduction techniques** on image data using:
- Principal Component Analysis (PCA)
- t-Distributed Stochastic Neighbor Embedding (t-SNE)

The goal is to understand how these techniques behave on:
- Structured data (handwritten digits)
- Complex real-world data (human faces)

---

## 📊 Datasets Used
- MNIST Dataset (Handwritten Digits)
- Labeled Faces in the Wild (Face Dataset)

---

## 🎯 Objectives
- Apply PCA for dimensionality reduction
- Visualize data in 2D space
- Reconstruct images using PCA
- Compare classification performance (with vs without PCA)
- Apply t-SNE for advanced visualization
- Analyze differences between structured and complex datasets

---

## ⚙️ Methodology

### 1️⃣ Data Preprocessing
- Normalized image data
- Reduced dataset size for faster computation (especially for t-SNE)

### 2️⃣ PCA Implementation
- Applied PCA on both datasets
- Analyzed explained variance
- Selected optimal number of components (95% variance)

### 3️⃣ Visualization
- 2D PCA projection
- t-SNE visualization for non-linear structure

### 4️⃣ Reconstruction
- Reconstructed images using reduced PCA components
- Compared original vs reconstructed images

### 5️⃣ Classification
- Trained SVM classifier:
  - Without PCA
  - With PCA
- Compared accuracy and performance

### 6️⃣ Performance Analysis
- Accuracy comparison
- Training time comparison
- Reconstruction error (MSE)

---

## 📈 Results & Observations

### 🔹 PCA (Explained Variance)
- Faces capture high variance in fewer components initially
- MNIST distributes variance more gradually

### 🔹 Visualization
- PCA:
  - MNIST → clear clusters
  - Faces → overlapping clusters
- t-SNE:
  - Better cluster separation than PCA
  - Captures non-linear patterns effectively

### 🔹 Reconstruction
- MNIST:
  - Retains structure even after compression
- Faces:
  - Loses fine details due to complexity

### 🔹 Classification
- PCA reduces dimensionality and training time
- Slight drop or similar accuracy depending on components used

---

## 💡 Key Insights
- PCA works well for structured datasets like digits
- Faces require more components due to higher variability
- t-SNE provides better visualization but is not suitable for modeling
- Dimensionality reduction involves a trade-off between:
  - Accuracy
  - Speed
  - Information loss

---

## ⚠️ Limitations
- PCA is a linear method (cannot capture complex patterns)
- t-SNE is computationally expensive
- t-SNE cannot be used for reconstruction or classification

---

## 🛠 Tech Stack
- Python
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow (for MNIST)

---

##  Sample Outputs
- PCA variance graphs
- 2D projections (PCA & t-SNE)
- Reconstruction comparisons
- Accuracy comparison plots

---

## 🚀 Conclusion
This project demonstrates how dimensionality reduction techniques behave differently depending on dataset complexity. While PCA is effective for reducing dimensions and improving efficiency, advanced methods like t-SNE provide deeper insights into data structure.

---

## 📌 Future Improvements
- Compare with UMAP
- Build interactive visualization (Streamlit)
- Apply deep learning-based dimensionality reduction (Autoencoders)

---

## ⭐ If you found this useful, feel free to star the repo!
