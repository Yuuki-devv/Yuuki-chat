<div align="center">

<img src="https://files.catbox.moe/hxqfag.jpg" width="120" style="border-radius:50%;" />

# 💜 Yuuki Chat App
### Blue Archive × AI Chatbot

*Ngobrol santai bareng Yuuki, kapanpun kamu mau.*

![Blue Archive](https://img.shields.io/badge/Blue%20Archive-Yuuki-7eaaff?style=for-the-badge)
![HTML](https://img.shields.io/badge/Built%20With-HTML%20Only-orange?style=for-the-badge)
![No Framework](https://img.shields.io/badge/Framework-None-brightgreen?style=for-the-badge)

</div>

---

<div align="center">
  <img src="https://files.catbox.moe/8zod03.jpg" width="80%" style="border-radius:16px; opacity:0.85;" />
  <br/>
  <sub><i>Background yang digunakan di aplikasi</i></sub>
</div>

---

## 📋 Daftar Isi

- [Cara Pakai](#-cara-pakai)
- [Konfigurasi](#️-konfigurasi)
- [Fitur](#-fitur)
- [Fullscreen](#-fullscreen)
- [Ganti Gambar](#️-ganti-gambar)
- [Kustomisasi Karakter](#-kustomisasi-karakter)
- [Catatan Penting](#-catatan-penting)

---

## 🚀 Cara Pakai

### Option A — Buka Langsung (Lokal)
```
1. Download file yuuki.html
2. Buka di browser (Chrome direkomendasikan)
3. Selesai — tidak perlu install apapun
```

### Option B — Host Online *(Direkomendasikan untuk HP)*

Upload ke salah satu platform gratis berikut:

| Platform | Cara | Link |
|----------|------|------|
| **Netlify Drop** | Drag & drop file langsung | [app.netlify.com/drop](https://app.netlify.com/drop) |
| **GitHub Pages** | Push ke repo, aktifkan Pages | [pages.github.com](https://pages.github.com) |
| **Vercel** | Import repo atau drag & drop | [vercel.com](https://vercel.com) |

> ⚠️ Hosting online **wajib** jika ingin fullscreen berfungsi di Android.

---

## ⚙️ Konfigurasi

Buka `yuuki.html`, cari bagian ini di dalam `<script>`:

```js
const TOKEN    = '230623'                          // ← Ganti token kamu
const API_BASE = 'https://cynix.tokopanel.my.id'  // ← Jangan diubah
```

| Variable | Fungsi | Ubah? |
|----------|--------|-------|
| `TOKEN` | Token autentikasi API | ✅ Ganti dengan milikmu |
| `API_BASE` | URL server API | ❌ Jangan diubah |

---

## ✨ Fitur

### 💬 Chat AI
Ngobrol natural dengan Yuuki. Dia merespons sesuai konteks waktu — malam hari lebih santai, jam kerja lebih semangat.

### 🖼️ Kirim Pap
Ketik salah satu:
- `"kirim pap dong"`
- `"foto dong"`
- `"kasih pap"`

Yuuki otomatis cari foto dari Pinterest. Swipe kiri/kanan untuk navigasi.

### 🌙 Time-Aware Responses

| Waktu | Trigger | Respons Yuuki |
|-------|---------|---------------|
| 22:00 – 05:00 | Sebut kata begadang / malam | Negur dengan caring |
| 08:00 – 17:00 | Sebut kata gabut / nganggur | Semangatin buat produktif |

### ⛶ Mode Fullscreen
Tombol di pojok kanan header. Detail di bagian [Fullscreen](#-fullscreen).

### 💾 Penyimpanan Sesi
Chat tersimpan selama tab masih terbuka via `sessionStorage`. Ditutup = reset.

### 📱 Mobile Friendly
Responsif di semua ukuran layar. Swipe untuk navigasi foto pap.

---

## ⛶ Fullscreen

```
⛶ Fullscreen  →  Masuk fullscreen
✕ Exit        →  Keluar fullscreen
Tekan Esc     →  Keluar fullscreen (tombol otomatis reset)
```

**Kenapa harus klik dulu?**  
Browser memblokir fullscreen otomatis saat halaman pertama dibuka — ini kebijakan keamanan browser, bukan bug.

**Kenapa perlu hosting untuk Android?**  
File via `file://` punya izin terbatas. Hosting online (`https://`) memberikan akses penuh ke Fullscreen API.

---

## 🖼️ Ganti Gambar

Cari dan ganti dua URL ini di bagian CSS:

```css
/* Background halaman */
background: url('https://files.catbox.moe/8zod03.jpg') center/cover;

/* Foto profil Yuuki */
background: url('https://files.catbox.moe/hxqfag.jpg') center/cover;
```

**Cara upload gambar baru:**
1. Upload ke [catbox.moe](https://catbox.moe) atau [imgur.com](https://imgur.com)
2. Copy link gambar
3. Tempel ke URL di atas

---

## 🎭 Kustomisasi Karakter

Cari variabel `AI_LOGIC` di script:

```js
const AI_LOGIC = `Kamu adalah Yuuki dari Blue Archive.
Cewek dengan rambut biru, berkacamata, anggota Abydos High School.
Kepribadianmu: serius tapi sesekali kaku lucu...`
```

Bisa diubah:
- Nama & lore karakter
- Cara bicara (formal, santai, campur bahasa Inggris)
- Topik yang boleh/tidak dibahas

---

## 📝 Catatan Penting

| Hal | Keterangan |
|-----|------------|
| **Chat hilang** | Normal — sessionStorage reset saat tab ditutup |
| **Foto pap gagal** | Cek koneksi atau coba lagi |
| **AI tidak merespons** | Pastikan token aktif dan koneksi stabil |
| **Fullscreen tidak jalan** | Gunakan Chrome 80+ dan host online |
| **Lag di HP lama** | Efek blur berat di GPU — normal |

---

## 📁 Struktur File

```
📦 Yuuki Chat App
 ├── yuuki.html    ← Semua-dalam-satu (HTML + CSS + JS)
 └── README.md     ← Dokumentasi ini
```

---

<div align="center">
  <img src="https://files.catbox.moe/hxqfag.jpg" width="60" style="border-radius:50%;opacity:0.7;" />
  <br/><br/>
  <sub>Made with 💙 &nbsp;|&nbsp; Yuuki © Blue Archive / Nexon</sub>
</div>
