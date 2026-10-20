# Panduan Roda Pintar Samudera

Permainan suku kata untuk murid Tahap 1. Semua kod berada dalam **satu fail**, `index.html`, tanpa pustaka luar.

Aliran permainan:
1. **Skrin Mula**: murid isi nama dan kelas.
2. **Roda Impian**: putar roda untuk mendapat satu perkataan.
3. **Bina Perkataan**: seret suku kata yang betul ke kotak jawapan. Ada 4 suku kata perangkap.
4. **Misi Sebutan**: tekan butang 🎤 dan sebut perkataan itu. Sebutan yang betul memberi +10 markah.

---

## Langkah 1: Rakam audio

Rakam setiap suku kata dan setiap perkataan penuh. Simpan rakaman dalam format **`.m4a`**, contohnya dengan aplikasi Voice Memos di iPhone atau perakam suara di Android. Namakan setiap fail **tepat** seperti senarai di bawah, menggunakan **huruf kecil semua**.

**37 fail suku kata:**
```
ba.m4a    bin.m4a   bis.m4a   bu.m4a
cang.m4a  ci.m4a    cin.m4a   da.m4a
dang.m4a  das.m4a   dom.m4a   gar.m4a
gung.m4a  he.m4a    ja.m4a    jam.m4a
kul.m4a   kun.m4a   kut.m4a   lang.m4a
lem.m4a   pa.m4a    pan.m4a   pet.m4a
pi.m4a    pu.m4a    put.m4a   ren.m4a
rum.m4a   sam.m4a   sang.m4a  so.m4a
tan.m4a   tang.m4a  tim.m4a   tong.m4a
yung.m4a
```

**20 fail perkataan penuh:**
```
garpu_penuh.m4a     lembu_penuh.m4a     kunci_penuh.m4a
panda_penuh.m4a     timba_penuh.m4a     jambatan_penuh.m4a
bintang_penuh.m4a   cincin_penuh.m4a    sampan_penuh.m4a
rendang_penuh.m4a   biskut_penuh.m4a    tandas_penuh.m4a
rumput_penuh.m4a    cangkul_penuh.m4a   dompet_penuh.m4a
pisang_penuh.m4a    sotong_penuh.m4a    payung_penuh.m4a
helang_penuh.m4a    jagung_penuh.m4a
```

Jumlah: **57 fail**. Letakkan semuanya dalam satu folder bernama **`audio`**.

Petua: pastikan setiap rakaman pendek, jelas, dan tidak bermula dengan senyap yang panjang.

---

## Langkah 2: Muat naik ke GitHub

1. Daftar akaun percuma di https://github.com jika belum ada.
2. Tekan **+** di penjuru kanan atas, kemudian **New repository**.
   - **Repository name:** contohnya `roda-pintar-samudera`
   - Pilih **Public** (GitHub Pages percuma hanya untuk repo Public).
   - Tekan **Create repository**.
3. Di halaman repo baharu, tekan pautan **uploading an existing file**.
4. Seret fail **`index.html`** dan **folder `audio`** ke halaman itu. Folder `audio` mesti diseret sebagai folder, bukan fail-failnya satu per satu, supaya struktur folder dikekalkan.
5. Tekan **Commit changes**.

Struktur akhir repo mesti begini:
```
roda-pintar-samudera/
├── index.html
└── audio/
    ├── ba.m4a
    ├── ...
    └── jagung_penuh.m4a
```

---

## Langkah 3: Aktifkan laman web (GitHub Pages)

1. Di repo anda, pergi ke **Settings → Pages**.
2. Di bahagian **Build and deployment**:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` dan folder `/ (root)`, kemudian tekan **Save**.
3. Tunggu 1–2 minit, kemudian muat semula halaman itu. Pautan permainan akan muncul, biasanya:
   `https://NAMA-PENGGUNA-ANDA.github.io/roda-pintar-samudera/`

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
| 1 | Garpu | gar + pu |
| 2 | Lembu | lem + bu |
| 3 | Kunci | kun + ci |
| 4 | Panda | pan + da |
| 5 | Timba | tim + ba |
| 6 | Jambatan | jam + ba + tan |
| 7 | Bintang | bin + tang |
| 8 | Cincin | cin + cin |
| 9 | Sampan | sam + pan |
| 10 | Rendang | ren + dang |
| 11 | Biskut | bis + kut |
| 12 | Tandas | tan + das |
| 13 | Rumput | rum + put |
| 14 | Cangkul | cang + kul |
| 15 | Dompet | dom + pet |
| 16 | Pisang | pi + sang |
| 17 | Sotong | so + tong |
| 18 | Payung | pa + yung |
| 19 | Helang | he + lang |
| 20 | Jagung | ja + gung |

---

## Menukar perkataan sendiri (pilihan)

Semua tetapan berada di bahagian atas `<script>` dalam `index.html`. Di GitHub, buka `index.html`, tekan ikon pensel ✏️ (Edit), buat perubahan, kemudian tekan **Commit changes**. Cara paling mudah mencari bahagian yang betul ialah dengan **Ctrl+F**.

Setiap perkataan mesti dikemas kini di **3 tempat**:

**1. `SENARAI_PERKATAAN`**: perkataan dan pecahan suku katanya.
```js
{ word: "Lembu", syl: ["lem", "bu"] },
```
- `word` bermula dengan huruf besar. Suku kata ditulis dalam huruf kecil.
- Perkataan 3 suku kata juga disokong, contohnya `syl: ["ke", "re", "ta"]`.
- Disyorkan 12–24 perkataan supaya tulisan pada roda masih mudah dibaca.

**2. `audioMap`**: fail audio bagi setiap suku kata dan perkataan.
```js
"lem": "audio/lem.m4a",
"bu": "audio/bu.m4a",
"Lembu": "audio/lembu_penuh.m4a",
```
- Suku kata yang sama hanya perlu ditulis **sekali** walaupun muncul dalam beberapa perkataan.
- Pastikan fail `.m4a` itu wujud dalam folder `audio`.

**3. `iconMap`**: gambar bagi setiap perkataan.
```js
"Lembu": "🐄",
```
- Nilainya boleh berupa **emoji** (contoh `"🐘"`) atau **laluan gambar** (contoh `"gambar/lembu.png"`). Jika guna gambar, muat naik gambar itu ke folder `gambar`.

Perhatian semasa menyunting:
- Setiap baris dalam senarai mesti diakhiri dengan **koma**, kecuali baris terakhir.
- Jangan padam tanda `{ }`, `[ ]` atau `" "`.
- Jika permainan tidak dapat dibuka selepas disunting, biasanya ada koma atau tanda petik yang tertinggal.

### Tetapan lain (pilihan)
- `JUMLAH_DISTRAKTOR = 4`: bilangan suku kata perangkap di skrin Bina Perkataan.
- `AMBANG_KETEPATAN = 0.75`: tahap ketepatan sebutan yang diterima, dari 0.75 (lebih bertoleransi) hingga 0.90 (lebih ketat).
- `MARKAH_BETUL = 10`: markah bagi setiap sebutan yang betul.
