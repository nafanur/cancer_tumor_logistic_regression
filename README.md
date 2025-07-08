# cancer_tumor_logistic_regression
- **Tujuan:** analisis klasifikasi dengan regresi logistik biner PySpark untuk memprediksi apakah seorang pasien terdiagnosis tumor ganas atau jinak berdasarkan fitur-fitur morfologi sel.
- **Data:** https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset

- **Variabel Data:**
  variabel prediktor (X): 
1. radius_mean: Rata-rata jari-jari inti sel.
2. texture_mean: Rata-rata variasi tekstur permukaan sel.
3. area_mean: Rata-rata luas inti sel.
4. perimeter_mean: Rata-rata keliling inti sel.
5. compactness_mean: Ukuran kekompakan bentuk sel, biasanya dihitung dari perbandingan antara perimeter dan area.
6. radius_se: Standar deviasi (error) dari ukuran jari-jari inti sel.
7. area_se: Standar deviasi (error) dari ukuran luas inti sel.
8. perimeter_se: Standar deviasi (error) dari ukuran keliling inti sel.
9. radius_worst: Nilai maksimum dari jari-jari inti sel pada kondisi terburuk.
10. texture_worst: Nilai maksimum dari tekstur permukaan inti sel pada kondisi terburuk.
11. area_worst: Nilai maksimum dari luas inti sel pada kondisi terburuk.
12. concavity_worst: Nilai maksimum dari tingkat cekungan bentuk inti sel.
13. symmetry_worst: Nilai maksimum dari tingkat simetri bentuk inti sel.

variabel respon (Target Y): `diagnosis`
Nilainya terdiri dari dua kelas:
'M' = Malignant (ganas)
'B' = Benign (jinak)

- **Hasil Evaluasi Model**:
 Nilai AUC pada ROC curve yang dihasilkan adalah 0.99. Menurut (Hosmer et al., 2013), nilai AUC 0,99 menunjukkan bahwa model regresi logistik biner memiliki kemampuan luar biasa (outstanding) untuk membedakan kelas (tumor ganas dan jinak).
