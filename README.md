1. Tambahkan fitur Ubah PIN
a.	Tambahkan opsi ‘Ubah Pin’ pada menu utama 
Kode pada bagian showMenu(Account account) telah diperbarui untuk menampilkan opsi "Ubah PIN" sebagai pilihan nomor 5. Saat pengguna memilih opsi ini, metode changePin(account) akan dipanggil.

b.	Buat mdeo dalam kelas Account untuk mengubah PIN, yaitu: changePin()
Menambahkan method dikelas Account dengan nama changePin untuk menu ubah pin

c.	Dalam method tersebut lakukan hal berikut:
i.	Verifikasi PIN lama
ii.	Minta nasabah memasukkan PIN baru dua kali
iii.	Validasi bahwa kedua input PIN baru cocok
iv.	Perbarui PIN jika validasi berhasil
 

2.	Validasi Saldo Minimal pada saat penarikan
a.	Modifikasi fitur penarikan sehingga nasabah harus menyisakan saldo minimal setelah penarikan dilakukan. Misal, saldo minial adalah Rp50,000-

b.	Langkah-langkah:
i.	Tentukan saldo minimal, tambahkan konstanta MINIMUM_BALANCE dalam kelas Account

menambahkan konstanta MINIMUM_BALANCE dalam kelas Account untuk menentukan saldo minimal. Misalnya, jika saldo minimal ditetapkan sebesar Rp50,000, tambahkan baris berikut di dalam kelas Account:
ii.	Modifikasi methode execute() dalam kelas Withdrawal untuk memeriksa apakah saldo setelah penarikan tidak kuran dari saldo minimal
 
menambahkan logika dalam metode execute() di kelas Withdrawal untuk memeriksa apakah saldo setelah penarikan tidak kurang dari saldo minimal. Kelas Withdrawal harus mengimplementasikan metode execute() dan memverifikasi apakah penarikan tersebut bisa dilakukan berdasarkan saldo minimal yang ditentukan.






iii.	Jika saldo tidak mencukupi, tampilkan pesan kesalahan
 


