# Baba Movement × Hardwork Copy — GitHub / Netlify

Cabang ini khusus untuk website **Fotokopi & Percetakan**. Cabang `main` BabaLanja tidak boleh diubah oleh installer ini.

**Status:** repositori pendukung sudah disiapkan; sumber produksi V5 masih berada pada paket ZIP yang disediakan dalam percakapan ChatGPT. Jangan hubungkan cabang ini ke Netlify sebelum file V5 diunggah ke cabang ini. Tidak ada kredensial API di repository.

**Proyek Netlify:** https://app.netlify.com/projects/baba-movement-dokumen-ai

**Konfigurasi yang diperlukan saat mengaktifkan:**
- `DATABASE_URL` dan `SESSION_SECRET`: sudah disimpan pada proyek Netlify, jangan memasukkan ulang ke GitHub.
- `JAGEL_API_KEY` dan `OPENAI_API_KEY`: harus dibuat sendiri pada masing-masing layanan dan disimpan sebagai environment variables di Netlify.
- `HWC_ADMIN_PASSWORD`: buat sendiri, minimal 12 karakter.
- `ENABLE_JAGEL_PAYMENTS=false` sampai pembayaran saldo sungguhan berhasil diuji.

**Langkah otomatis dari ZIP:** Jalankan `DEPLOY_NETLIFY_WINDOWS.bat` setelah mengekstrak paket V5 terbaru pada komputer dengan Node.js. Installer menguji kode, menghubungkan ke proyek Netlify yang benar, dan melakukan deploy dengan login/izin Netlify. Untuk sinkronisasi GitHub, gunakan `UPLOAD_KE_GITHUB_WINDOWS.bat` yang mengunggah ke cabang khusus ini tanpa mengubah `main`.

Setelah source masuk ke cabang ini, hubungkan Netlify melalui **Project configuration → Continuous deployment → Link repository** dan pilih `babalanja77/babalanjasep2025`, cabang `hardwork-copy-netlify`. Setelah itu setiap push ke cabang produksi terpilih dapat memicu build otomatis.

**Jangan menganggap login Jagel, push APK, atau debit saldo sudah aktif** sebelum diuji dengan akun asli.
