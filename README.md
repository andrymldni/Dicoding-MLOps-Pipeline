## Submission 1: Deteksi Stres pada Manusia Berdasarkan Riwayat Curhatan

Nama: Andry Syva Maldini<br>
Username dicoding: andrymldni

<p align="center">
  <img src="https://github.com/user-attachments/assets/e43f8938-ab79-4020-89a6-794bba9b2401" alt="dataset-cover" width="700" height="350">
</p>

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Human Stress Detection](https://www.kaggle.com/datasets/itslakhvir/human-stress-detection) |
| Masalah | Masalah yang diangkat dalam proyek ini adalah mendeteksi tingkat stres atau kecemasan dari teks curhatan pribadi seseorang. Banyak individu yang mengekspresikan kekhawatiran atau perasaan cemas melalui tulisan, dan proyek ini berupaya untuk mengidentifikasi pola bahasa yang menunjukkan tingkat stres tersebut. |
| Solusi machine learning | Solusi machine learning yang akan dibangun adalah sebuah model klasifikasi berbasis teks yang dapat memprediksi apakah curhatan yang diberikan mengandung indikasi stres atau tidak. Model ini akan memproses teks input, mengidentifikasi pola kecemasan, dan mengeluarkan prediksi berupa label biner: 1 (mengandung stres) atau 0 (tidak mengandung stres). |
| Metode pengolahan | Pada dataset Human Stress Prediction, terdapat tujuh fitur, namun dalam proyek ini hanya fitur teks dan label yang akan digunakan. Fitur lainnya akan dihapus, setelah itu data akan dibagi menjadi data pelatihan dan evaluasi dengan rasio 80:20. Selain itu, fitur teks akan diubah menjadi huruf kecil, dan labelnya akan diubah menjadi bentuk integer. |
| Arsitektur model | Arsitektur model yang diterapkan adalah model embedding, yang terdiri dari layer vectorization, diikuti oleh layer embedding dengan dimensi embedding sebesar 16. Selanjutnya, digunakan layer AveragePooling1D karena data berbentuk teks, kemudian layer dense dengan 64 dan 32 neuron menggunakan aktivasi ReLU dan sigmoid, karena model ini akan melakukan klasifikasi antara dua label. Fungsi loss yang digunakan adalah binary_crossentropy, dengan optimizer Adam dan metrik BinaryAccuracy. |
| Metrik evaluasi | Metrik evaluasi yang diterapkan meliputi ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, serta BinaryAccuracy. |
| Performa model | Hasil evaluasi model menunjukkan AUC sebesar 83%, dengan jumlah contoh sebanyak 575, BinaryAccuracy mencapai 74%, dan loss sebesar 1.456. Selain itu, terdapat 86 False Negatives, 62 False Positives, 214 True Negatives, dan 213 True Positives. Model yang telah dikembangkan masih memiliki potensi untuk ditingkatkan, mengingat BinaryAccuracy masih di bawah 80%. |

<p align="center">
  <img src="https://github.com/user-attachments/assets/0973a95f-24ad-44aa-906d-2115f50d5d9c" alt="dicoding">
</p>
