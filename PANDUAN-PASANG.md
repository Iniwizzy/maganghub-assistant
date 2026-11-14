# Panduan pasang MagangHub Assistant v1.0.0

Ekstensi browser untuk peserta magang MagangHub: tulis laporan harian dari 1 kalimat dengan Gemini, isi ke form dengan 1 klik, dan dapat pengingat lewat notifikasi browser dan WhatsApp.

> **Pakai Microsoft Edge?** Pasang langsung dari [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/peknndhcccnefhjjafddhchdihemhkca): klik **Get**, lalu **Add extension**. Tanpa Developer mode, dan versi baru masuk sendiri. Setelah itu lanjut ke [langkah 6](#6-atur-api-key-gemini-sekali-saja).
>
> Langkah 1–5 di bawah untuk **Google Chrome** (belum ada di Chrome Web Store), atau untuk Edge kalau kamu memilih pasang manual.

## Yang dibutuhkan

- Laptop atau PC dengan **Google Chrome** atau **Microsoft Edge** versi 116 ke atas (Windows, macOS, atau Linux). Tidak bisa dipasang di HP.
- Akun peserta di [monev.maganghub.kemnaker.go.id](https://monev.maganghub.kemnaker.go.id).
- API key Gemini gratis dari Google AI Studio (langkah 6).
- Opsional: WhatsApp, untuk pengingat yang tetap masuk walau laptop mati.

## 1. Download

Unduh **`maganghub-assistant-v1.0.0.zip`** (34,7 KB).

Untuk memastikan file tidak berubah (opsional), cocokkan SHA-256-nya:

```
1cca1d0d11be3fcf93cda94a44eb62c4f28f69457f1b01b81e1f3cdb2542989d
```

Di Windows, buka PowerShell di folder Downloads lalu jalankan:

```powershell
Get-FileHash .\maganghub-assistant-v1.0.0.zip -Algorithm SHA256
```

## 2. Ekstrak ke folder tetap

- **Windows:** klik kanan file zip → **Extract All…** → pilih folder yang tidak akan kamu hapus, misalnya `Documents\MagangHub Assistant`.
- **macOS:** klik dua kali file zip, lalu pindahkan foldernya ke `Documents`.

Penting:

- **Jangan hapus atau pindahkan folder ini** setelah ekstensi dipasang. Browser menjalankan ekstensi langsung dari folder ini.
- Di dalam folder itu harus langsung ada file `manifest.json`.

## 3. Buka halaman ekstensi

Ketik alamat ini di address bar, lalu tekan Enter:

| Browser | Alamat |
|---|---|
| Chrome | `chrome://extensions` |
| Edge | `edge://extensions` |

## 4. Nyalakan Developer mode

- **Chrome:** sakelar **Developer mode** di kanan atas halaman.
- **Edge:** sakelar **Developer mode** di panel kiri, bagian bawah.

Kalau browser-mu berbahasa Indonesia, namanya kurang lebih **Mode pengembang**.

## 5. Muat ekstensinya

1. Klik **Load unpacked** (di browser berbahasa Indonesia, namanya kurang lebih *Muat yang belum dibuka*).
2. Pilih folder dari langkah 2, yaitu folder yang berisi `manifest.json`.
3. **MagangHub Assistant** muncul di daftar ekstensi.
4. Sematkan ikonnya supaya mudah dibuka: klik ikon puzzle (Ekstensi) di toolbar, lalu klik ikon pin di samping MagangHub Assistant.

## 6. Atur API key Gemini (sekali saja)

1. Buka [aistudio.google.com/apikey](https://aistudio.google.com/apikey), login dengan akun Google, klik **Create API key**, lalu salin key-nya.
2. Klik ikon MagangHub Assistant → tab **Pengaturan** → tempel key → **Simpan & tes koneksi**.
3. Pilih model: **Cepat** (disarankan), **Hemat**, atau **Terbaik**.

API key hanya disimpan di browser-mu dan hanya dikirim ke Google Gemini.

## 7. Pakai setiap hari

1. Login ke MagangHub dan buka form laporan hari ini.
2. Klik ikon MagangHub Assistant → tab **Laporan** → tulis 1 kalimat tentang kegiatanmu → **Buat laporan dengan AI**.
3. Periksa dan edit tiga kolomnya, lalu klik **Isi ke form MagangHub**.
4. Di halaman MagangHub, baca ulang, **centang pernyataan, lalu klik Simpan dan Kirim sendiri**. Ekstensi tidak pernah mengirim laporan untukmu.

## 8. Pengingat (opsional)

- **Notifikasi browser:** tab **Pengingat** → pilih jam (bawaan 11:30, 13:30, 16:30, bisa tambah sampai 3 jam lain) dan hari. Notifikasi muncul selama browser terbuka.
- **WhatsApp:** tab **Pengingat** → **Hubungkan WhatsApp**. WhatsApp terbuka dengan pesan `DAFTAR <kode>`, tinggal kirim. Bot membalas "Terhubung!".
  - Balas **sudah** untuk menghentikan pengingat hari itu.
  - Balas **STOP** untuk berhenti total, **MULAI** untuk menyalakan lagi.

Pengingat berhenti sendiri setelah laporan hari itu terkirim.

## Update ke versi baru

Versi dari Edge Add-ons update sendiri. Untuk versi yang dipasang manual:

1. Download zip versi baru.
2. Ekstrak ke **folder yang sama** dengan langkah 2, timpa file lamanya. Folder harus sama supaya pengaturan dan sambungan WhatsApp tidak hilang.
3. Buka halaman ekstensi, lalu klik tombol muat ulang (ikon panah melingkar) di kartu MagangHub Assistant.

## Pindah ke versi toko

Sudah pasang manual di Edge? Pindah ke versi toko supaya update datang otomatis:

1. Kalau WhatsApp terhubung: popup → **Pengingat** → **Putuskan dan hapus nomor dari server**.
2. Hapus versi manual di halaman ekstensi (**Remove**), lalu hapus foldernya.
3. Pasang dari [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/peknndhcccnefhjjafddhchdihemhkca), isi API key lagi, dan hubungkan WhatsApp lagi bila perlu.

Jangan pasang dua versi sekaligus, karena pengingat bisa muncul dobel. Di Chrome belum ada versi toko, jadi tetap pakai versi manual.

## Menghapus ekstensi

1. Kalau WhatsApp terhubung, putuskan dulu (lihat di atas) supaya nomormu terhapus dari server.
2. Klik **Remove** di halaman ekstensi.
3. Hapus folder hasil ekstrak.

## Masalah umum

| Masalah | Solusi |
|---|---|
| "Manifest file is missing or unreadable" | Folder yang dipilih salah. Pilih folder yang langsung berisi `manifest.json`. |
| Ekstensi hilang atau error setelah folder dipindah | Ekstrak lagi ke folder yang sama, lalu klik muat ulang di halaman ekstensi. |
| Browser menampilkan peringatan tentang ekstensi mode pengembang | Itu peringatan biasa untuk ekstensi yang dipasang manual. Tutup peringatannya; jangan pilih menonaktifkan ekstensi. |
| Tes koneksi Gemini gagal | Salin ulang API key. Kalau pesannya soal kuota atau model sibuk, coba pilihan **Hemat** atau tunggu sebentar. |
| **Isi ke form** tidak mengisi | Pastikan form laporan hari ini terbuka di tab yang aktif. Kalau tetap gagal, pakai tombol **Salin** di tiap kolom. |
| Notifikasi tidak muncul | Izinkan notifikasi untuk browser di pengaturan sistem (Windows: Settings → System → Notifications). |

## Privasi

Ringkasnya: API key dan teks laporan disimpan di browser-mu. Teks aktivitas hanya dikirim ke Google Gemini saat kamu menekan **Buat laporan dengan AI**. Nomor WhatsApp hanya disimpan kalau kamu menghubungkan WhatsApp, dan bisa dihapus kapan saja. Ekstensi hanya berjalan di monev.maganghub.kemnaker.go.id dan tidak membaca cookie, password, atau tab lain.

Kebijakan privasi lengkap: https://script.google.com/macros/s/AKfycbxAWKs0sjiFAL4atwmuKfHf1KgiOPyplGoEfVtnBrTnen7JtFloSUxN4flhgJOt1i_v5A/exec?page=privacy

## Tentang

Ekstensi independen, **tidak berafiliasi dengan Kemnaker atau MagangHub**. Pastikan isi laporan sesuai dengan kegiatanmu yang sebenarnya sebelum dikirim.

Dibuat oleh [@wwizzyyy](https://www.instagram.com/wwizzyyy/). Versi 1.0.0, dirilis 14 November 2026.
