# 📘 Judul Proyek
*Klasifikasi Penyakit Tanaman Kedelai Menggunakan Machine Learning dan Deep Learning*

## 👤 Informasi
- **Nama:** Satria Bagus Al Imanu
- **Repo:** https://github.com/SatriaBagus313/soybean-ml-project
- **Video:** https://www.youtube.com/watch?v=APqRxn0c080&feature=youtu.be

---

# 1. 🎯 Ringkasan Proyek
Proyek ini bertujuan untuk melakukan klasifikasi penyakit tanaman kedelai menggunakan dataset Soybean Small dari UCI Machine Learning Repository.
Tahapan yang dilakukan meliputi:
- Pemahaman masalah dan eksplorasi data
- Data preparation dan preprocessing
- Pembangunan 3 model klasifikasi: **Baseline, Advanced Machine Learning,** dan **Deep Learning**
- Evaluasi performa model dan pemilihan model terbaik

---

# 2. 📄 Problem & Goals
**Problem Statements:**  
- Bagaimana cara mengklasifikasikan penyakit tanaman kedelai berdasarkan fitur-fitur kategorikal yang tersedia?
- Model apa yang memberikan performa terbaik untuk klasifikasi penyakit pada dataset Soybean Small?

**Goals:**  
- Membangun sistem klasifikasi penyakit tanaman kedelai berbasis machine learning dan deep learning.
- Membandingkan performa beberapa model dan menentukan model terbaik berdasarkan metrik evaluasi.

---
## 📁 Struktur Folder
```
project/
│
├── data/                   # Dataset (tidak di-commit, download manual)
│
├── notebooks/              # Jupyter notebooks
│   └── ML_Project.ipynb
│
├── src/                    # Source code
│   
├── models/                 # Saved models
│   ├── model_baseline.pkl
│   ├── model_rf.pkl
│   └── model_cnn.h5
│
├── images/                 # Visualizations
│   └── r
│
├── requirements.txt        # Dependencies
├── .gitignore
└── README.md
```
---

# 3. 📊 Dataset
- **Sumber:** https://archive.ics.uci.edu/dataset/91/soybean+small
- **Jumlah Data:** 47 data
- **Jumlah Fitur:** 35 fitur
- **Target Kelas:** Penyakit tanaman kedelai 
- **Tipe:** Seluruh fitur dan target bersifat **kategorikal**

### Fitur Utama
| Fitur | Deskripsi |
|leaf-shape|Bentuk daun|
|leaf-color|Warna daun|
|leaf-spot|Kondisi bercak pada daun|
|plant-growth|Pertumbuhan tanaman|

---

# 4. 🔧 Data Preparation
Tahapan data preparation yang dilakukan:
- **Data Cleaning:** menangani missing value dan memastikan tidak ada data duplikat
- **Transformasi Data:** encoding fitur kategorikal agar dapat diproses oleh model
- **Data Splitting:** membagi data menjadi data training dan testing

---

# 5. 🤖 Modeling
Model yang digunakan dalam proyek ini:
- **Model 1 – Baseline:** Naive Bayes
- **Model 2 – Advanced ML:** Random Forest Classifier
- **Model 3 – Deep Learning:** Multilayer Perceptron (MLP)

---

# 6. 🧪 Evaluation
**Metrik:** Accuracy, Precision, Recall, dan F1-Score

### Hasil Singkat
| Model | Score | Catatan |
|-------|--------|---------|
| Baseline (Naive Bayes) | 0.75 | Model sederhana sebagai pembanding |
| Advanced (Random Forest) | 0.85 | Mampu menangkap hubungan non-linear |
| Deep Learning (MLP) | 0.89 | Performa terbaik |

---

# 7. 🏁 Kesimpulan
- **Model terbaik:** Multilayer Perceptron (MLP)
- **Alasan:** Memiliki nilai accuracy dan F1-score tertinggi dibandingkan model lainnya
- **Insight penting:** Model deep learning lebih efektif dalam mempelajari hubungan kompleks antar fitur kategorikal pada dataset Soybean Small

---

# 8. 🔮 Future Work
- [ ] Tambah data  
- [ ] Tuning model  
- [ ] Coba arsitektur DL lain  
- [ ] Deployment  

---

# 9. 🔁 Reproducibility
Gunakan environment:
Python 3.10
numpy==1.24.3
pandas==2.0.3
scikit-learn==1.3.0
matplotlib==3.7.2
seaborn==0.12.2
tensorflow==2.14.0

