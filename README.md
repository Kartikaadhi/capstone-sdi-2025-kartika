# Capstone Project SDI 2025

## Analisis Aspirasi Generasi Muda melalui Fenomena #KaburAjaDulu dengan Bantuan IBM Granite

---

### Deskripsi Proyek

Fenomena #KaburAjaDulu mencerminkan keresahan nyata generasi muda terhadap berbagai isu seperti ekonomi, pendidikan, dan sosial di Indonesia. Dalam proyek ini, saya mencoba memahami aspirasi mereka lewat opini-opini publik yang tersebar di media sosial dan menganalisisnya menggunakan model bahasa besar (LLM) dari IBM Granite. Hasil dari analisis ini diharapkan bisa menjadi masukan yang relevan bagi pemerintah dan institusi terkait.

---
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12wQMrD5G2jjy6br9GsOtAsglg1Dkq4ye?usp=sharing)

### Tujuan Proyek

- Menggali opini publik yang berkaitan dengan #KaburAjaDulu
- Mengelompokkan aspirasi ke dalam kategori: Ekonomi, Sosial, Pendidikan, Budaya
- Memberikan rekomendasi kebijakan berdasarkan hasil analisis
- Membandingkan klasifikasi dari AI dengan penilaian manusia

---

### Teknologi yang Digunakan

| Komponen    | Detail                                              |
| ----------- | --------------------------------------------------- |
| Platform    | Google Colab                                        |
| Model AI    | IBM Granite 3.3-8B Instruct via Replicate API       |
| Bahasa      | Python + LangChain                                  |
| Visualisasi | Matplotlib, Wordcloud                               |
| Output      | Ringkasan, klasifikasi, rekomendasi, tabel evaluasi |

---

### Dataset

- Sumber: opini publik seputar #KaburAjaDulu (dikumpulkan secara manual)
- Format: CSV / DataFrame (`clean_text`)
- Contoh: "kerja penuh koneksi dan nepotisme", "pendidikan mahal dan susah diakses"

---

### Ringkasan Output Granite

```
Aspirasi Utama:
- Ekonomi: Ingin penghasilan layak dan kerja tanpa nepotisme
- Pendidikan: Biaya mahal, akses internet terbatas
- Sosial: Lingkungan kerja yang toksik dan tidak manusiawi

Klasifikasi:
- Ekonomi: 2 aspirasi
- Pendidikan: 1 aspirasi
- Sosial: 2 aspirasi

Rekomendasi:
1. Perluasan akses internet dan beasiswa vokasi
2. Perbaikan regulasi ketenagakerjaan dan pembangunan industri yang sehat
```

---

### Analisis Top Kata

| Top Kata Harapan | Frekuensi |
| ---------------- | --------- |
| ingin            | 2         |
| layak            | 1         |
| berharap         | 1         |
| kesejahteraan    | 1         |

| Top Kata Kekecewaan | Frekuensi |
| ------------------- | --------- |
| tidak               | 2         |
| kabur               | 1         |
| keluar              | 1         |
| mahal               | 1         |

---

### Perbandingan Manual vs LLM

| Opini Publik                                                             | Manual Kategori | LLM Kategori |
| ------------------------------------------------------------------------ | --------------- | ------------ |
| pendidikan di sini mahal dan gak semua daerah punya akses internet capek | Pendidikan         | Pendidikan   |
| bukan benci negara sendiri cuma pengen hidup yang lebih manusiawi        | Ekonomi      | Sosial       |
| lingkungan kerja toxic banget senioritas berlebihan                      | Sosial          | Sosial       |

> 📌 *Beberapa perbedaan muncul antara klasifikasi manual dan hasil dari LLM. Ini justru menarik karena memberikan sudut pandang baru dan membuka diskusi tentang bagaimana AI memahami konteks sosial.*

---

### Penjelasan Lengkap dari Granite

1. **Opini:** "pendidikan mahal dan akses internet terbatas"\
   **LLM Kategori:** Pendidikan\
   *Penjelasan:* Model menganggap ini sebagai masalah pendidikan karena menyebut biaya sekolah dan keterbatasan infrastruktur digital.

2. **Opini:** "ingin hidup manusiawi"\
   **LLM Kategori:** Sosial\
   *Penjelasan:* Fokus opini ini adalah pada kehidupan yang layak dan lebih manusiawi, sehingga masuk kategori sosial.

3. **Opini:** "lingkungan kerja toxic dan senioritas"\
   **LLM Kategori:** Sosial\
   *Penjelasan:* Karena menyangkut kondisi kerja yang tidak sehat dan struktur senioritas yang tidak seimbang, model menganggap ini sebagai isu sosial.

---

### Visualisasi

- Wordcloud Aspirasi
- Bar Chart Kategori Aspirasi
- Daftar Kata Harapan & Kekecewaan

---

### Insight Tambahan

Saya percaya bahwa banyak anak muda tidak benar-benar ingin meninggalkan negaranya. Mereka hanya ingin hidup yang lebih adil, lingkungan kerja yang sehat, dan kesempatan berkembang tanpa harus "kabur" ke tempat lain. Aspirasi ini menunjukkan betapa pentingnya peran negara dan institusi dalam menciptakan ruang hidup yang layak bagi generasi muda.

---

### Penulis

Kartika Adhi Ning Wulan Satunggal\
Program SDI 2025 – Capstone AI x IBM

---

### Lisensi

Proyek ini dibuat untuk pembelajaran dan refleksi sosial. Model Granite digunakan melalui Replicate API dan hanya untuk keperluan non-komersial.

