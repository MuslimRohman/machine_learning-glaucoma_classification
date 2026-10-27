# Klasifikasi Glaukoma pada Citra Retina Menggunakan MobileNetV3 dan MLP

**Machine Learning | Deep Learning | Computer Vision | Python**

## Deskripsi Proyek

Proyek ini bertujuan untuk mengembangkan model **klasifikasi glaukoma pada citra retina** menggunakan **MobileNetV3** sebagai *feature extractor* dan **Multilayer Perceptron (MLP)** sebagai *classifier*.

Penelitian menggunakan 2.417 citra retina dari tiga dataset, yaitu **Hillel-Yaffe Glaucoma Dataset, G1020, dan ORIGA**, untuk membedakan citra retina glaukoma dan non-glaukoma melalui pendekatan *transfer learning*.

## link dataset:

1. https://www.kaggle.com/datasets/bharathry/hillel-yaffe-dataset-for-glaucoma-detection/data
2. https://www.kaggle.com/datasets/arnavjain1/glaucoma-datasets

Dataset pertama yaitu Hillel-Yaffe Dataset for Glaucoma Detection berisi 747 citra fundus retina untuk deteksi glaucomatous optic neuropathy (GON). Dataset terdiri dari gambar retina dengan label GON+ (indikasi glaukoma) dan GON− (non-glaukoma), serta dilengkapi anotasi label glaukoma dan skor kualitas citra. Dataset memiliki ukuran sekitar 130 MB dengan format gambar .jpg. dengan beresolusi bervariasi.

Kemudian dataset kedua kami menggunakan dataset Glaucoma Datasets Kaggle yang terdiri dari dataset G1020 dan ORIGA yang memiliki resolusi 512 x 512 pixel. Dataset G1020 memiliki total 1020 citra retina dengan label 1 (glaukoma) dan 0 (non-glaukoma), serta ukuran dataset sekitar 53,2 MB. Sedangkan dataset ORIGA memiliki total 650 citra retina dengan label 1 (glaukoma) dan 0 (non-glaukoma), serta ukuran dataset sekitar 35 MB. Kedua dataset digunakan untuk menambah jumlah data dan variasi citra retina agar model dapat mempelajari pola glaukoma dengan lebih baik. Ketiga dataset tersebut kemudian digabungkan menjadi satu dataset utama sehingga total data yang digunakan dalam penelitian ini menjadi 2417 citra retina untuk proses pelatihan dan evaluasi model klasifikasi glaukoma.

## Tools & Libraries

- **Python** – Bahasa pemrograman utama.
- **PyTorch** – Pengembangan dan pelatihan model Deep Learning.
- **MobileNetV3** – Ekstraksi fitur citra retina.
- **MLP** – Klasifikasi glaukoma dan non-glaukoma.
- **OpenCV** – Preprocessing citra.
- **Albumentations** – Augmentasi citra.
- **Scikit-learn** – Pembagian dataset dan evaluasi model.

## Tahapan Proyek

1. **Data Preparation:** Menggabungkan dan membersihkan tiga dataset citra retina.
2. **Preprocessing:** Resize 224×224 piksel, ekstraksi *green channel*, dan peningkatan kontras menggunakan CLAHE.
3. **Data Augmentation:** Menerapkan flipping, rotation, cropping, dan transformasi citra lainnya.
4. **Feature Extraction:** Menggunakan MobileNetV3 untuk mengekstraksi karakteristik citra retina.
5. **Classification:** Melakukan klasifikasi menggunakan Multilayer Perceptron (MLP).
6. **Model Evaluation:** Mengevaluasi performa berdasarkan accuracy, precision, recall, F1-score, dan AUC.

## Hasil Evaluasi Model

| Metrik | Nilai |
|---|---|
| Accuracy | 0.7735 |
| Precision | 0.7652 |
| Recall | 0.6645 |
| F1-Score | 0.7113 |
| AUC | 0.8249 |

Model menunjukkan kemampuan klasifikasi yang cukup baik dengan nilai AUC sebesar **0.8249**, meskipun kemampuan mendeteksi seluruh kasus glaukoma masih perlu ditingkatkan.

## Struktur Repository

- `Hasil Proyek/` — Hasil akhir dan dokumentasi proyek.
  - `Final_Code_Kelompok_1.ipynb` — Notebook pemodelan dan evaluasi akhir.
  - `Laporan Final_Kelompok 1.docx.pdf` — Laporan akhir proyek.
  - `Final Project Poster A1_Kelompok 1.jpeg` — Poster hasil penelitian.
  - `Flowchart Penelitian Klasifikasi Glaukoma MobileNetV3 + MLP.jpg` — Diagram alur penelitian.
- `Kemajuan Proyek/` — Dokumentasi perkembangan proyek.
- `Proposal Proyek/` — Dokumen proposal penelitian.
- `Revisi Proyek/` — Kode dan dokumentasi hasil revisi.
- `README.md` — Dokumentasi repository.

## Anggota Tim

- **Muhammad Ramadhan Albaary Putra**
- **Muslim Fazlur Rohman**
- **Kafka Praya Firmansyah**

**Program Studi Sains Data | Universitas Negeri Surabaya | 2026**
