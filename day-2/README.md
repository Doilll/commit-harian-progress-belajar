# Dasar Kriptografi dalam Blockchain

Kriptografi adalah tulang punggung yang menjamin keamanan dan integritas data di blockchain. Ada tiga konsep utama yang perlu dipahami: **hash**, **public/private key**, dan **digital signatures**.

---

## 1. Hash (Fungsi Hash Kriptografi)

Fungsi hash kriptografi mengubah data apa pun menjadi serangkaian karakter alfanumerik dengan panjang tetap, disebut **nilai hash** atau **digest**.

**Karakteristik:**
- **Input Berubah, Output Sangat Berubah:** Perubahan kecil pada input menghasilkan hash yang sangat berbeda.
- **Satu Arah:** Tidak mungkin mengembalikan hash ke data asli.
- **Unik:** Hampir mustahil dua input berbeda menghasilkan hash yang sama.

**Peran di Blockchain:**
- Setiap blok memiliki nilai hash unik.
- Setiap blok menyimpan hash blok sebelumnya, membentuk rantai yang tidak bisa diubah.
- Perubahan data pada blok akan memutus rantai, sehingga upaya pemalsuan mudah terdeteksi.

---

## 2. Public/Private Key (Kunci Publik/Pribadi)

Sistem enkripsi asimetris ini mengamankan transaksi di blockchain. Setiap pengguna memiliki sepasang kunci:

- **Kunci Pribadi:** Rahasia, digunakan untuk menandatangani transaksi dan membuktikan kepemilikan.
- **Kunci Publik:** Dapat dibagikan, digunakan sebagai alamat dompet dan untuk menerima aset kripto.

**Cara Kerja:**
1. Pengguna menandatangani transaksi dengan kunci pribadi.
2. Penerima memverifikasi transaksi menggunakan kunci publik pengirim.

---

## 3. Digital Signatures (Tanda Tangan Digital)

Tanda tangan digital adalah aplikasi dari sistem kunci publik/pribadi, berupa kode matematis yang membuktikan:

- **Otentikasi:** Transaksi dibuat oleh pemilik kunci pribadi.
- **Integritas:** Data transaksi tidak diubah setelah ditandatangani.

**Proses:**
1. Membuat transaksi.
2. Data transaksi di-hash.
3. Hash dienkripsi dengan kunci pribadi menjadi tanda tangan digital.
4. Transaksi dan tanda tangan dikirim ke jaringan.
5. Node jaringan menggunakan kunci publik untuk memverifikasi tanda tangan dan integritas data.

---

## Kesimpulan

- **Hash:** Sidik jari unik untuk data.
- **Public/Private Key:** Identitas digital yang aman.
- **Digital Signatures:** Verifikasi dan keamanan transaksi.

Kombinasi ketiganya membuat blockchain aman dan terpercaya tanpa perantara.