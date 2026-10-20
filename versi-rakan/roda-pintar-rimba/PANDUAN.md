# Panduan Roda Pintar Rimba

Permainan suku kata untuk murid Tahap 1. Semua kod berada dalam **satu fail**, `index.html`, tanpa pustaka luar.

Aliran permainan:
1. **Skrin Mula**: murid isi nama dan kelas.
2. **Roda Impian**: putar roda untuk mendapat satu perkataan.
3. **Bina Perkataan**: seret suku kata yang betul ke kotak jawapan. Ada 4 suku kata perangkap.
4. **Misi Sebutan**: tekan butang 🎤 dan sebut perkataan itu. Sebutan yang betul memberi +10 markah.

---

## Langkah 1: Rakam audio

Rakam setiap suku kata dan setiap perkataan penuh. Simpan rakaman dalam format **`.m4a`**, contohnya dengan aplikasi Voice Memos di iPhone atau perakam suara di Android. Namakan setiap fail **tepat** seperti senarai di bawah, menggunakan **huruf kecil semua**.

**33 fail suku kata:**
```
ba.m4a   bo.m4a   bun.m4a  ci.m4a
du.m4a   gar.m4a  gi.m4a   hu.m4a
ja.m4a   jan.m4a  ka.m4a   kar.m4a
ke.m4a   ki.m4a   ko.m4a   ku.m4a
kul.m4a  lam.m4a  li.m4a   lo.m4a
pa.m4a   pi.m4a   ri.m4a   ro.m4a
rum.m4a  sa.m4a   su.m4a   ta.m4a
tam.m4a  tan.m4a  ti.m4a   to.m4a
tol.m4a
```

**20 fail perkataan penuh:**
```
gigi_penuh.m4a   kaki_penuh.m4a   topi_penuh.m4a
roti_penuh.m4a   sudu_penuh.m4a   tali_penuh.m4a
ciku_penuh.m4a   pasu_penuh.m4a   lori_penuh.m4a
duku_penuh.m4a   jarum_penuh.m4a  kolam_penuh.m4a
sabun_penuh.m4a  tikar_penuh.m4a  bakul_penuh.m4a
botol_penuh.m4a  hujan_penuh.m4a  ketam_penuh.m4a
pagar_penuh.m4a  hutan_penuh.m4a
```

Jumlah: **53 fail**. Letakkan semuanya dalam satu folder bernama **`audio`**.

Petua: pastikan setiap rakaman pendek, jelas, dan tidak bermula dengan senyap yang panjang.

---

## Langkah 2: Muat naik ke GitHub

1. Daftar akaun percuma di https://github.com jika belum ada.
2. Tekan **+** di penjuru kanan atas, kemudian **New repository**.
   - **Repository name:** contohnya `roda-pintar-rimba`
   - Pilih **Public** (GitHub Pages percuma hanya untuk repo Public).
   - Tekan **Create repository**.
3. Di halaman repo baharu, tekan pautan **uploading an existing file**.
4. Seret fail **`index.html`** dan **folder `audio`** ke halaman itu. Folder `audio` mesti diseret sebagai folder, bukan fail-failnya satu per satu, supaya struktur folder dikekalkan.
5. Tekan **Commit changes**.

Struktur akhir repo mesti begini:
```
roda-pintar-rimba/
├── index.html
└── audio/
    ├── ba.m4a
    ├── ...
    └── hutan_penuh.m4a
```

---

## Langkah 3: Aktifkan laman web (GitHub Pages)

1. Di repo anda, pergi ke **Settings → Pages**.
2. Di bahagian **Build and deployment**:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` dan folder `/ (root)`, kemudian tekan **Save**.
3. Tunggu 1–2 minit, kemudian muat semula halaman itu. Pautan permainan akan muncul, biasanya:
   `https://NAMA-PENGGUNA-ANDA.github.io/roda-pintar-rimba/`

Kongsikan pautan ini kepada murid.

---

## Langkah 4: Uji permainan

| Peranti | Pelayar yang disyorkan |
|---|---|
| Android | Google Chrome |
| iPhone / iPad | Safari (iOS 14.5 ke atas) |
| Komputer | Google Chrome |

1. Buka pautan dan isi nama dan kelas.
2. Putar roda, kemudian tekan kad perkataan. Bunyi perkataan penuh sepatutnya keluar.
3. Di skrin Bina Perkataan, tekan setiap kotak suku kata untuk mendengar bunyinya.
4. Di Misi Sebutan, tekan 🎤 dan **benarkan akses mikrofon**. Kali pertama, mungkin perlu tekan butang sekali lagi.

Perkara penting:
- **Mikrofon hanya berfungsi melalui pautan `https://`** (GitHub Pages). Ia tidak berfungsi jika `index.html` dibuka terus dari storan telefon.
- Jika halaman masih menunjukkan versi lama selepas dikemas kini, muat semula dengan **Ctrl+Shift+R** di komputer, atau tutup dan buka semula tab di telefon.
- Jika ada bunyi yang tidak keluar, semak ejaan nama fail. GitHub membezakan huruf besar dan kecil (`Gi.m4a` ≠ `gi.m4a`).

---

## Senarai perkataan dalam versi ini

| # | Perkataan | Suku kata |
|---|---|---|
| 1 | Gigi | gi + gi |
| 2 | Kaki | ka + ki |
| 3 | Topi | to + pi |
| 4 | Roti | ro + ti |
| 5 | Sudu | su + du |
| 6 | Tali | ta + li |
| 7 | Ciku | ci + ku |
| 8 | Pasu | pa + su |
| 9 | Lori | lo + ri |
| 10 | Duku | du + ku |
| 11 | Jarum | ja + rum |
| 12 | Kolam | ko + lam |
| 13 | Sabun | sa + bun |
| 14 | Tikar | ti + kar |
| 15 | Bakul | ba + kul |
| 16 | Botol | bo + tol |
| 17 | Hujan | hu + jan |
| 18 | Ketam | ke + tam |
| 19 | Pagar | pa + gar |
| 20 | Hutan | hu + tan |

---

## Menukar perkataan sendiri (pilihan)

Semua tetapan berada di bahagian atas `<script>` dalam `index.html`. Di GitHub, buka `index.html`, tekan ikon pensel ✏️ (Edit), buat perubahan, kemudian tekan **Commit changes**. Cara paling mudah mencari bahagian yang betul ialah dengan **Ctrl+F**.

Setiap perkataan mesti dikemas kini di **3 tempat**:

**1. `SENARAI_PERKATAAN`**: perkataan dan pecahan suku katanya.
```js
{ word: "Kaki", syl: ["ka", "ki"] },
```
- `word` bermula dengan huruf besar. Suku kata ditulis dalam huruf kecil.
- Perkataan 3 suku kata juga disokong, contohnya `syl: ["ke", "re", "ta"]`.
- Disyorkan 12–24 perkataan supaya tulisan pada roda masih mudah dibaca.

**2. `audioMap`**: fail audio bagi setiap suku kata dan perkataan.
```js
"ka": "audio/ka.m4a",
"ki": "audio/ki.m4a",
"Kaki": "audio/kaki_penuh.m4a",
```
- Suku kata yang sama hanya perlu ditulis **sekali** walaupun muncul dalam beberapa perkataan.
- Pastikan fail `.m4a` itu wujud dalam folder `audio`.

**3. `iconMap`**: gambar bagi setiap perkataan.
```js
"Kaki": "🦶",
```
- Nilainya boleh berupa **emoji** (contoh `"🐘"`) atau **laluan gambar** (contoh `"gambar/kaki.png"`). Jika guna gambar, muat naik gambar itu ke folder `gambar`.

Perhatian semasa menyunting:
- Setiap baris dalam senarai mesti diakhiri dengan **koma**, kecuali baris terakhir.
- Jangan padam tanda `{ }`, `[ ]` atau `" "`.
- Jika permainan tidak dapat dibuka selepas disunting, biasanya ada koma atau tanda petik yang tertinggal.

### Tetapan lain (pilihan)
- `JUMLAH_DISTRAKTOR = 4`: bilangan suku kata perangkap di skrin Bina Perkataan.
- `AMBANG_KETEPATAN = 0.75`: tahap ketepatan sebutan yang diterima, dari 0.75 (lebih bertoleransi) hingga 0.90 (lebih ketat).
- `MARKAH_BETUL = 10`: markah bagi setiap sebutan yang betul.
