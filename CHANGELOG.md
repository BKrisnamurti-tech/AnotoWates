# Perubahan

## 0.3.0

**Penting:** proyek `.anoproj` yang sudah disimpan oleh 0.3.0 memakai format skema 2 dan tidak bisa dibuka oleh 0.2.0 (versi lama menolaknya dengan pesan "perbarui aplikasi", bukan merusak data kerja tim). Proyek dari 0.2.0 tetap terbuka di 0.3.0.

### Baru
- Bilah menu di editor (Berkas, Edit, Tampilan, Bantuan) dan menu klik kanan untuk gambar dan kelas.
- Tahap **Review** dengan jumlah per status dan validasi seluruh dataset di latar belakang.
- **Cocokkan folder gambar**: gambar yang dipindah atau diganti nama ditemukan lewat isinya (SHA-256).
- Kerja tim: **Bagi tugas ke anotator** dan **Gabungkan paket anotator** dengan pilihan per konflik, gambar pratinjau, dan rincian kelas di tiap sisi.
- Ekstraksi video, crop gambar, dan ganti nama & format kini di tampilan baru, dengan pratinjau dan progres.
- Proyek terakhir bisa dibuka lewat menu ⋯ / klik kanan: tampilkan di folder, hapus dari daftar, atau hapus proyek (ke Recycle Bin, gambar tidak ikut terhapus).
- Ganti nama proyek dan anotator, Simpan sebagai, mode fokus (F11), sembunyikan anotasi (O), zoom ke objek (Z).
- Huruf Inter dan Plus Jakarta Sans ikut di aplikasi (tanpa internet), dengan skala ukuran teks yang seragam.
- Judul jendela menampilkan nama proyek atau alat yang terbuka.
- Catatan galat di `data\logs\anotowates.log` untuk dilampirkan saat melapor masalah.

### Lebih cepat dan hemat
- Menyimpan satu editan hanya menulis gambar itu: 0,1 detik, bukan 13 detik, di proyek 20.000 gambar.
- RAM aplikasi di layar awal turun dari ±730 MB menjadi ±90 MB.
- Membuka proyek besar lebih cepat (20.000 gambar × 8 objek: 16 → 10 detik) dan menampilkan "Membuka proyek…".
- Memulai ekspor tidak lagi membekukan editor (5,8 → 0,1 detik).

### Perbaikan
- Editan terakhir tidak hilang saat jendela ditutup; aplikasi bertanya dulu bila ekspor, alat berkas, validasi, atau pencocokan folder masih berjalan.
- Simpan yang gagal (disk penuh, berkas terkunci) tidak lagi menghilangkan editan; editor tetap di gambar itu dan mengirim ulang.
- Paket yang dikirim ulang setelah anotator lanjut bekerja tidak lagi menimbulkan konflik palsu; gambar yang sudah dikeluarkan dari proyek tidak ditambahkan kembali; kelas yang diganti nama setelah tugas dibagi tidak menjadi ganda; ID kelas yang dihapus tidak dipakai ulang.
- Bagi tugas kini semua-atau-tidak-sama-sekali: bila satu paket gagal ditulis, tidak ada paket setengah jadi dan proyek tidak berubah.
- Penanda waktu perubahan selalu naik, sehingga dua editan cepat tidak tercatat sebagai satu.
- Tata letak di layar 1280×720: tombol panel kanan tidak terpotong, label tombol "Enter" pas, "Memuat gambar…" tidak tertinggal di alat Crop.
- Pelat nomor kendaraan di foto layar awal disamarkan.
