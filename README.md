# Stunting Prediction with Machine Learning

## Tentang Dataset
Dataset Stunting ini mencakup atribut demografis dan terkait kesehatan yang bertujuan untuk memprediksi secara diagnostik apakah seorang pasien menderita stunting berdasarkan pengukuran diagnostik. Dataset mencakup informasi tentang Gender, Age, Birth Weight, Birth Length, Body Weight, Body Length, Breastfeeding, dan Stunting. Dataset ini memberikan data faktor-faktor yang berkontribusi pada Stunting serta memfasilitasi pengembangan model prediktif untuk penilaian risiko dan strategi pencegahan.

Keterangan Variabel
Stunting: Kondisi gagal tumbuh pada anak balita akibat kekurangan gizi kronis terutama dalam 1000 Hari Pertama Kehidupan (HPK).
Gender: Jenis Kelamin
Age: Usia
Birth Weight: Berat badan anak saat lahir.
Birth Length: Panjang badan anak saat lahir
Body Weight: Berat badan anak saat diukur
Body Length: Panjang badan anak saat diukur
Breastfeeding: ASI eksklusif yang diberikan kepada anak 6 bulan pertama


## Kesimpulan
1. Random Forest (RF) Random Forest menunjukkan performa yang sangat baik dan seimbang di seluruh metrik evaluasi, dengan akurasi sebesar 94.08%, precision 92.47%, recall 88.91%, dan F1-score 90.54%. Model ini unggul dalam hal presisi, menjadikannya pilihan tepat untuk kasus di mana kesalahan prediksi positif (false positive) perlu diminimalkan. Random Forest juga menunjukkan stabilitas yang tinggi dan cocok untuk digunakan dalam lingkungan produksi.

2. Decision Tree (DT) Decision Tree juga menunjukkan performa yang sangat kompetitif dengan Random Forest, mencatat akurasi 94.08%, precision 89.97%, recall 92.69%, dan F1-score 91.23%. Model ini memiliki nilai recall tertinggi di antara semua model, menjadikannya sangat andal dalam mendeteksi kasus positif. Selain itu, struktur model yang mudah diinterpretasi memberikan nilai tambah dalam konteks transparansi dan explainability.

3. K-Nearest Neighbors (KNN) Model KNN mencatat akurasi 86.95%, dengan precision 82.89%, recall 73.82%, dan F1-score 76.99%. Meskipun lebih rendah dibanding DT dan RF, model ini tetap menunjukkan performa yang layak. Namun, recall yang relatif rendah menunjukkan bahwa model masih cenderung meleset dalam mengidentifikasi kelas positif. Model ini dapat dipertimbangkan untuk kasus dengan kebutuhan komputasi ringan dan data berukuran kecil.

4. Support Vector Machine (SVM) SVM mencatat akurasi 83.20%, precision 80.58%, recall 61.84%, dan F1-score 64.37%. Performa recall yang rendah menunjukkan keterbatasan model dalam mendeteksi kelas positif, yang dapat menjadi kendala pada masalah klasifikasi yang sensitif terhadap kesalahan tipe II (false negatives).

5. Naive Bayes (NB) Naive Bayes merupakan model dengan performa paling rendah di antara lima model yang diuji, dengan akurasi 82.83%, precision 74.47%, recall 66.56%, dan F1-score 68.97%. Meskipun ringan dan cepat, model ini kurang mampu menangkap kompleksitas data secara optimal, sehingga kurang direkomendasikan sebagai model utama dalam skenario ini.

## Rekomendasi
Berdasarkan hasil evaluasi, Random Forest dan Decision Tree merupakan model yang paling optimal, dengan performa tinggi dan seimbang di semua metrik. Keduanya sangat direkomendasikan untuk digunakan lebih lanjut, baik dalam proses deployment maupun pengambilan keputusan. Jika diperlukan interpretasi model yang lebih transparan, Decision Tree dapat menjadi pilihan utama. Sebaliknya, jika stabilitas dan akurasi menjadi prioritas, maka Random Forest adalah opsi terbaik.
