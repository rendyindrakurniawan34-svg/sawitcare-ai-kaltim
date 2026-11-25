# SawitCare AI - Deteksi Dini Hama & Penyakit Kelapa Sawit di Kalimantan Timur

## Summary
SawitCare AI adalah ide aplikasi mobile berbasis AI untuk membantu petani kecil kelapa sawit di Kalimantan Timur (khususnya sekitar Samarinda) mendeteksi dini hama dan penyakit dari foto daun dan buah sawit.

## The Problem
Petani kecil di Kaltim sering terlambat mendeteksi Ganoderma, ulat api, dan defisiensi hara. Akses ke ahli agronomi terbatas dan mahal. Kerugian bisa 30-40% hasil panen.

## My AI Idea - The Solution
1. Petani foto daun/buah yang mencurigakan.
2. Model Computer Vision (CNN EfficientNet) klasifikasi: Sehat, Ganoderma, Ulat Api, Kekurangan Kalium.
3. Beri rekomendasi tindakan dalam Bahasa Indonesia sederhana.
4. Peta sebaran hama anonim per kecamatan (privacy-preserving).

## Data
Sumber: Dataset publik PlantVillage + MPOB + foto lapangan dari petani mitra (dengan izin). Kebutuhan MVP ~5000 gambar per kelas. Mitigasi bias: data mencakup kondisi cahaya hujan/panas Kaltim dan HP entry-level.

## Technology
Model: Transfer Learning EfficientNet-B0 / MobileNetV3 untuk on-device inference (TFLite) karena sinyal di kebun jelek. Stack: Python, TensorFlow.

## Ethics & Risks
- False Negative: tampilkan confidence score, saran konsultasi ke penyuluh jika <80%.
- Privacy: tidak menyimpan GPS presisi, hanya kecamatan.
- Copyright: foto tetap milik petani.

## Impact
Membantu >10.000 petani kecil di Kaltim meningkatkan yield 15-20% dan mengurangi pestisida berlebihan.

---
Project for Elements of AI - Building AI course - Your AI Idea. Created by Rendy Indra from Samarinda.
