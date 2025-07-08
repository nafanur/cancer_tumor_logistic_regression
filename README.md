# cancer_tumor_logistic_regression
- **Tujuan:** analisis klasifikasi dengan regresi logistik biner PySpark untuk memprediksi apakah seorang pasien terdiagnosis tumor ganas atau jinak berdasarkan fitur-fitur morfologi sel.
- **Data:** https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset

- **Variabel Data:**
  variabel prediktor (X): 
| Nama Variabel      | Penjelasan singkat                                                    |
| ------------------ | --------------------------------------------------------------------- |
| `radius_mean`      | Rata-rata jari-jari inti sel                                          |
| `texture_mean`     | Rata-rata variasi tekstur permukaan sel                               |
| `area_mean`        | Rata-rata luas inti sel                                               |
| `perimeter_mean`   | Rata-rata keliling inti sel                                           |
| `compactness_mean` | Ukuran kekompakan bentuk sel (perbandingan antara perimeter dan area) |
| `radius_se`        | Standar error dari jari-jari                                          |
| `area_se`          | Standar error dari luas                                               |
| `perimeter_se`     | Standar error dari keliling                                           |
| `radius_worst`     | Nilai maksimum dari jari-jari pada kondisi terburuk                   |
| `texture_worst`    | Nilai maksimum dari tekstur sel pada kondisi terburuk                 |
| `area_worst`       | Nilai maksimum dari luas inti sel                                     |
| `concavity_worst`  | Nilai maksimum dari cekungan bentuk sel                               |
| `symmetry_worst`   | Nilai maksimum dari simetri bentuk sel                                |

variabel respon (Target Y): `diagnosis`
Nilainya terdiri dari dua kelas:
'M' = Malignant (ganas)
'B' = Benign (jinak)

- **Hasil Evaluasi Model**:
 Nilai AUC pada ROC curve yang dihasilkan adalah 0.99. Menurut (Hosmer et al., 2013), nilai AUC 0,99 menunjukkan bahwa model regresi logistik biner memiliki kemampuan luar biasa (outstanding) untuk membedakan kelas (tumor ganas dan jinak).
