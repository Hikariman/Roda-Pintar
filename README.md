# Roda Pintar Angkasa 🚀

Permainan suku kata bertema angkasa lepas untuk murid sekolah rendah (Tahap 1).
Seluruh permainan berada dalam **satu fail**: `index.html` (HTML + CSS + JavaScript, tanpa pustaka luar).

## Aliran
1. **Skrin Mula** – isi Nama & Kelas.
2. **Roda Impian** – putar roda 20 perkataan.
3. **Bina Perkataan** – seret suku kata ke kotak jawapan (sokong tetikus & skrin sentuh).
4. **Misi Sebutan** – tekan butang mikrofon dan sebut perkataan untuk membawa roket melepasi halangan (+10 markah).

## Audio sendiri
Fail audio (format `.m4a`) berada dalam folder `audio/` dan sunting objek `audioMap` di bahagian atas `<script>` dalam `index.html`.
Kesan bunyi juga boleh ditukar melalui `sfxMap`, dan ikon/gambar melalui `iconMap`.

## Arahan suara 🔊
Butang bulat 🔊 di penjuru kanan atas memainkan arahan suara (untuk murid yang belum boleh membaca).
Muat naik fail ini ke folder `audio/` (nama mesti tepat, huruf kecil, tiada ruang):

| Fail | Bila dimainkan |
|---|---|
| `panduan_penggunaan.m4a` | Skrin Mula + pop-up tutorial Roda Impian |
| `gabung_suku_kata.m4a` | Bina Perkataan + pop-up tutorialnya |
| `uji_rakaman_roket.m4a` | Misi Sebutan + pop-up tutorialnya |

Laluan fail boleh diubah dalam objek `arahanMap` dalam `index.html`.

## Penting untuk pengecaman suara
- Buka permainan melalui **https://** (contoh GitHub Pages) – mikrofon tidak berfungsi jika fail dibuka terus dari storan telefon.
- Android: gunakan Google Chrome. iPhone: Safari (iOS 14.5 ke atas).
- Ketepatan sebutan dilaraskan melalui `AMBANG_KETEPATAN` (0.75 – 0.90).
