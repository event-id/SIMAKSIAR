# Implementasi referensi Simak Siar Vol. 36

## Perubahan
- Halaman kategori tiket memakai dua produk pada referensi: Festival Rp75.000 dan Bundle Ticket (T-Shirt + Tiket Festival) Rp210.000.
- Kedua kategori ditandai ON SALE.
- Tombol Pilih Tiket ditempatkan di sisi kiri area bawah card; kontrol jumlah +/- ditampilkan setelah kategori dipilih.
- Tombol Beli Tiket tetap nonaktif sebelum jumlah pilihan minimal satu; setelah dipilih, alur menuju form.html.
- Formulir menyimpan format order yang kompatibel dengan data yang dibaca qris.html.
- QRIS menampilkan proses fullscreen selama 3 menit dan kemudian menuju success.html.
- Halaman success menampilkan status menunggu verifikasi pembayaran.

## Catatan transaksi yang sangat penting
Timer 3 menit hanya menunjukkan proses pengiriman/penanganan data. Timer, unggahan bukti, atau email terkirim tidak membuktikan dana sudah masuk. Karena ZIP ini tidak menyediakan integrasi verifikasi bank/payment gateway yang dapat diverifikasi, halaman akhir menyatakan **Menunggu verifikasi pembayaran panitia**, bukan pembayaran lunas. Status lunas harus ditetapkan oleh admin atau callback backend tepercaya.

## Pemeriksaan yang dilakukan
Pemeriksaan statis terhadap file HTML, skrip inline, referensi aset, dan kontrak penyimpanan lokal. Pengujian transaksi live dan pengujian browser end-to-end tidak diklaim karena membutuhkan layanan eksternal dan lingkungan browser yang terhubung.
