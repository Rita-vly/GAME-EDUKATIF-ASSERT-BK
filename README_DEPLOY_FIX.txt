ASSERT — DEPLOY CANDIDATE

Base: ASSERT game asli. Perbaikan hanya menambahkan satu data engine di akhir index.html dan mempertahankan backend functions yang sudah ada.

Perbaikan data:
- Student ID internal unik; nama tetap hanya nama tampilan.
- Data pusat Netlify Blobs dikunci berdasarkan Student ID.
- Siswa >36 tetap diterima; 36 adalah target kelas, bukan batas penyimpanan.
- Jawaban, pilihan/interaksi, dan draft refleksi disimpan.
- Progress misi berurutan.
- Control Room membaca data pusat.
- Delete siswa menggunakan Student ID dan diverifikasi setelah DELETE.
- Tidak ada S1–S8 dan tidak ada script eksternal baru.

GitHub:
1. Ganti index.html.
2. Ganti netlify/functions/assert-data.mjs.
3. Pertahankan netlify.toml dan package.json.
4. Commit ke branch yang terhubung ke Netlify.
5. Jangan hapus file lama sampai tes live selesai.

Environment variable tetap: ASSERT_BK_CODE=ASSERT-BK (atau nilai yang saat ini dipakai deployment).
