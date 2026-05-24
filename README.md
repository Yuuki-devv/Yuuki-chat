# 💜 Yuuki — Blue Archive Chat App

Aplikasi chat AI berbasis karakter Yuuki dari Blue Archive. Dibangun dengan HTML/CSS/JS murni, tanpa framework tambahan.

---

## 🚀 Cara Pakai

### 1. Buka langsung di browser
Cukup buka file `yuuki.html` di browser. Tidak perlu server atau install apapun.

### 2. Host online (direkomendasikan)
Untuk fitur fullscreen dan akses dari HP, upload ke:
- [GitHub Pages](https://pages.github.com/)
- [Netlify Drop](https://app.netlify.com/drop) — drag & drop file langsung
- [Vercel](https://vercel.com/)

---

## ⚙️ Konfigurasi

Buka `yuuki.html`, cari bagian `// ── CONFIG ──` di script:

```js
const TOKEN    = '230623'           // ← Ganti dengan token API kamu
const API_BASE = 'https://cynix.tokopanel.my.id'
```

| Variable   | Keterangan |
|------------|------------|
| `TOKEN`    | Token dari cynix.tokopanel.my.id |
| `API_BASE` | Base URL API (jangan diubah kecuali punya server sendiri) |

---

## ✨ Fitur

| Fitur | Keterangan |
|-------|------------|
| 💬 Chat AI | Percakapan natural dengan karakter Yuuki Blue Archive |
| 🖼️ Kirim Pap | Ketik "kirim pap dong" → otomatis cari foto Yuuki dari Pinterest |
| 🌙 Time-aware | Yuuki akan tegur kalau kamu begadang, atau semangatin kalau jam kerja |
| ⛶ Fullscreen | Tombol fullscreen di header (butuh klik manual, wajib di browser) |
| 💾 Session | Chat tersimpan selama tab masih buka (sessionStorage) |
| 📱 Mobile-friendly | Responsive, support swipe untuk navigasi foto |

---

## 🖼️ Cara Ganti Gambar

Di bagian CSS dan JS, ada dua URL gambar:

```
Background : https://files.catbox.moe/8zod03.jpg
Profile    : https://files.catbox.moe/hxqfag.jpg
```

Ganti URL tersebut dengan link gambar milikmu. Bisa upload ke [catbox.moe](https://catbox.moe/) atau [imgur.com](https://imgur.com/) lalu copy link-nya.

---

## ⛶ Tentang Fullscreen

- Tombol **⛶ Fullscreen** ada di header kanan atas
- Klik sekali → masuk fullscreen
- Klik lagi → keluar fullscreen
- **Catatan:** Chrome tidak mengizinkan fullscreen otomatis saat halaman buka — harus dipicu oleh klik user
- Di Android, fullscreen bekerja optimal jika file dihost online (bukan `file://`)

---

## 📁 Struktur File

```
yuuki.html   ← File utama, semua-dalam-satu (HTML + CSS + JS)
README.md    ← Dokumentasi ini
```

---

## 🔧 Kustomisasi Karakter

Cari variabel `AI_LOGIC` di script untuk mengubah kepribadian Yuuki:

```js
const AI_LOGIC = `Kamu adalah Yuuki dari Blue Archive. ...`
```

Edit teks di sana sesuai selera. Bisa ubah nama, sifat, cara bicara, dll.

---

## 📝 Catatan

- Chat **tidak tersimpan** setelah tab ditutup (menggunakan sessionStorage)
- Fitur pap mengambil gambar dari Pinterest via API — hasil tergantung koneksi
- Semua request AI melewati API cynix.tokopanel.my.id — pastikan token aktif
