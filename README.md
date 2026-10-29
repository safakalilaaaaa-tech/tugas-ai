# Studi Ablasi RNN, LSTM, GRU vs ANN untuk Prediksi Trafik Seluler Milan

Tugas Workshop Deep Learning — Teknik Telekomunikasi ITERA.

<!-- Ganti seluruh isian bertanda [ ... ] di bawah. Hapus komentar ini. -->

## Kelompok

| Peran | Nama | NIM |
|---|---|---|
| Ketua | [Safa Kalila] | [124400020] |
| Anggota | [Deola Stefani] | [124400095] |
| Anggota | [Danisha Dwi Kartika] | [124400074] |

- **Kelas:** [RB]
- **Lokasi kelompok:** [0] — [Stazione Centrale] (digit terakhir NIM terkecil)
- **Laporan:** [`laporan-latex/main.pdf` atau `laporan-typst/main.pdf`]

## Cara Menjalankan

```bash
uv sync
uv run jupyter lab
```

Buka `tugas_ablasi.ipynb`, isi `LOKASI_KELOMPOK`, lalu jalankan semua sel. Semua run tercatat di `hasil/ablasi.csv`.

Perangkat yang kami pakai: [Laptop Axioo dengan prosesor AMD Ryzen 5 (CPU)], total waktu training: [76] menit.

## Ringkasan Hasil

[Eksperimen ini membandingkan model ANN, RNN, LSTM, dan GRU untuk memprediksi trafik seluler di Milan. Berdasarkan hasil pengujian konfigurasi terbaik, model GRU memperoleh test MAE sebesar 220,3, RNN sebesar 224,5, LSTM sebesar 245,6, dan ANN sebesar 269,4. Dengan demikian, GRU menghasilkan nilai MAE terendah di antara keempat model pada pengujian tersebut. Hasil generalisasi pada lokasi Stazione Centrale menunjukkan bahwa performa model dapat berubah ketika diterapkan pada lokasi yang berbeda.]

## Struktur

```
tugas_ablasi.ipynb      notebook eksperimen (di-commit beserta output)
data/                   data trafik per jam (Duomo + 10 lokasi tugas)
hasil/                  CSV seluruh run, tabel, dan grafik
laporan-latex/ atau laporan-typst/   sumber laporan + PDF
```

## Data

Telecom Italia Big Data Challenge (Barlacchi dkk., 2015, *Scientific Data*, lisensi ODbL), versi per jam dari Zhang dkk. (INFOCOM 2021). Disiapkan oleh pengajar di repo [mctosima/dl-workshop](https://github.com/mctosima/dl-workshop).
