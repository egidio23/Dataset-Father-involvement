# 🧠 Father Involvement Scale (FIS) Dataset

## 📘 Overview
Dataset ini merupakan hasil penelitian yang bertujuan untuk mengukur tingkat keterlibatan ayah (*father involvement*) pada siswa yang tinggal bersama ayah kandung. Skala ini dikembangkan berdasarkan teori **Doherty** yang mencakup tiga aspek utama, yaitu **engagement**, **accessibility**, dan **responsibility**.  
Data dikumpulkan menggunakan instrumen psikologi model **Guttman** dengan dua pilihan jawaban (“Ya” dan “Tidak”).

---

## 📊 Dataset Description

**Dataset Name:** Father Involvement Scale (FIS)  
**Purpose:** Mengidentifikasi tingkat keterlibatan ayah berdasarkan persepsi anak terhadap perilaku dan peran ayah dalam kehidupan sehari-hari.  
**Instrument Type:** Skala model **Guttman**  
**Response Options:** Dua pilihan jawaban — **“Ya”** dan **“Tidak”**  
**Sampling Technique:** *Purposive sampling* (non-probability sampling) dengan kriteria siswa yang **tinggal bersama ayah kandung**.  
**Total Respondents:** 195 siswa  
- 38 siswa dengan peran *father involvement* **rendah**  
- 157 siswa dengan peran *father involvement* **tinggi**

**Data Collection Method:**  
Data dikumpulkan menggunakan kuesioner psikologi dengan 10 item pernyataan yang terdiri atas pernyataan *favorable* dan *unfavorable*. Responden diminta memilih satu dari dua opsi (“Ya” atau “Tidak”) sesuai dengan kondisi yang dialaminya. Tidak ada jawaban yang benar atau salah.

---

## 🧾 Father Involvement Scale — Item Pertanyaan

| No | Pernyataan | Jawaban |
|----|-------------|---------|
| 1 | Ayah sering mengajak saya mengunjungi tempat yang saya suka setiap kali ada waktu luang | Ya / Tidak |
| 2 | Saya sering bertanya kepada Ayah tentang pelajaran yang sulit dimengerti | Ya / Tidak |
| 3 | Meskipun sedang sibuk, Ayah selalu bersedia untuk merawat saya ketika saya sedang sakit | Ya / Tidak |
| 4 | Saya sering berbagi cerita dengan Ayah tentang keseharian saya | Ya / Tidak |
| 5 | Ketika saya sedang berada di luar rumah, Ayah sering mengabari saya melalui handphone | Ya / Tidak |
| 6 | Ketika akan beraktivitas di luar rumah, saya selalu meminta izin kepada Ayah | Ya / Tidak |
| 7 | Ayah selalu mengajak saya berdiskusi mengenai masalah atau kesulitan yang sedang saya alami | Ya / Tidak |
| 8 | Saya merasa aman ketika berada di dekat Ayah | Ya / Tidak |
| 9 | Ayah membelikan semua peralatan sekolah yang memang saya butuhkan | Ya / Tidak |
| 10 | Ayah mengajak saya berdiskusi terkait hal-hal yang boleh saya lakukan dan hal-hal yang harus saya hindari | Ya / Tidak |

---

## 📁 File Information

**Format File:** `.csv` atau `.xlsx`  
**Struktur Kolom:**
- `id_responden` — Nomor unik responden  
- `item_1` hingga `item_10` — Jawaban untuk setiap pernyataan  
- `total_score` — Jumlah jawaban “Ya”  
- `kategori` — Klasifikasi peran father involvement (*tinggi* / *rendah*)  

📂 [Download Dataset](./data/father_involvement.csv)

---

## 💻 How to Use

Contoh penggunaan dataset menggunakan Python (pandas):

```python
import pandas as pd

# Load dataset
data = pd.read_csv('father_involvement.csv')

# Tampilkan 5 baris pertama
print(data.head())

# Statistik dasar
print(data.describe())
