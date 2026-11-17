# MagangHub Assistant

Ekstensi browser untuk peserta magang MagangHub: tulis laporan harian dari 1 kalimat dengan AI (Gemini, atau model lain lewat OpenRouter), isi ke form dengan 1 klik, dan dapat pengingat lewat notifikasi browser dan WhatsApp.

**[Pasang di Edge (Microsoft Edge Add-ons)](https://microsoftedge.microsoft.com/addons/detail/peknndhcccnefhjjafddhchdihemhkca)** · **[Download untuk Chrome (zip v1.1.0, 45,7 KB)](https://github.com/Iniwizzy/maganghub-assistant/releases/latest/download/maganghub-assistant-v1.1.0.zip)** · [Panduan pasang](PANDUAN-PASANG.md) · [Halaman download](https://iniwizzy.github.io/maganghub-assistant/)

> **Edge:** pasang dari [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/peknndhcccnefhjjafddhchdihemhkca), tanpa Developer mode, update otomatis. **Chrome:** belum ada di Chrome Web Store, jadi pasang manual dengan langkah di bawah. Khusus laptop/PC.

## Pasang manual (Chrome)

1. Download zip, lalu ekstrak ke folder yang tidak akan kamu hapus.
2. Buka `chrome://extensions` atau `edge://extensions`, lalu nyalakan **Developer mode**.
3. Klik **Load unpacked**, pilih folder yang berisi `manifest.json`.
4. Klik ikon ekstensi → tab **Pengaturan** → tempel API key Gemini gratis dari [aistudio.google.com/apikey](https://aistudio.google.com/apikey). Atau pilih **OpenRouter** → **Hubungkan OpenRouter** untuk login dan memakai model lain.

Langkah lengkap, cara update, pindah ke versi toko, dan masalah umum ada di [PANDUAN-PASANG.md](PANDUAN-PASANG.md).

SHA-256 `maganghub-assistant-v1.1.0.zip`:

```
c6ebbbdb517954461080aea5adf7811497f37db3eacd9596a750ab176dde7993
```

## Privasi

API key, key OpenRouter, dan teks laporan disimpan di browser-mu. Teks aktivitas hanya dikirim ke penyedia AI yang kamu pilih saat kamu menekan Buat laporan dengan AI. Nomor WhatsApp hanya disimpan kalau kamu menghubungkan WhatsApp, dan bisa dihapus kapan saja dari popup. Kebijakan privasi lengkap: https://script.google.com/macros/s/AKfycbxAWKs0sjiFAL4atwmuKfHf1KgiOPyplGoEfVtnBrTnen7JtFloSUxN4flhgJOt1i_v5A/exec?page=privacy

---

Repo ini hanya berisi paket rilis dan panduannya. Ekstensi independen, **tidak berafiliasi dengan Kemnaker atau MagangHub**. Dibuat oleh [@wwizzyyy](https://www.instagram.com/wwizzyyy/).
