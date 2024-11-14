Tugas
1.	Tambahkan fitur Ubah PIN
a.	Tambahkan opsi ‘Ubah Pin’ pada menu utama
![image](https://github.com/user-attachments/assets/9921524b-07db-4941-b579-91fcb37d94d9)

Kode pada bagian showMenu(Account account) telah diperbarui untuk menampilkan opsi "Ubah PIN" sebagai pilihan nomor 5. Saat pengguna memilih opsi ini, metode changePin(account) akan dipanggil.

b.	Buat mdeo dalam kelas Account untuk mengubah PIN, yaitu: changePin()
 ![image](https://github.com/user-attachments/assets/7c45bb47-3d59-4099-8839-922daaecb6be)

Menambahkan method dikelas Account dengan nama changePin untuk menu ubah pin

c.	Dalam method tersebut lakukan hal berikut:
i.	Verifikasi PIN lama
ii.	Minta nasabah memasukkan PIN baru dua kali
iii.	Validasi bahwa kedua input PIN baru cocok
iv.	Perbarui PIN jika validasi berhasil
 ![image](https://github.com/user-attachments/assets/5fcd59e6-5a18-4b71-b72e-983b27eed8ee)


2.	Validasi Saldo Minimal pada saat penarikan
a.	Modifikasi fitur penarikan sehingga nasabah harus menyisakan saldo minimal setelah penarikan dilakukan. Misal, saldo minial adalah Rp50,000-
 ![image](https://github.com/user-attachments/assets/fb09b055-358a-4394-8db2-cb73b642384b)

b.	Langkah-langkah:
i.	Tentukan saldo minimal, tambahkan konstanta MINIMUM_BALANCE dalam kelas Account
 ![image](https://github.com/user-attachments/assets/499d552a-7514-4fcc-bd48-3d8aed95e86f)

menambahkan konstanta MINIMUM_BALANCE dalam kelas Account untuk menentukan saldo minimal. Misalnya, jika saldo minimal ditetapkan sebesar Rp50,000, tambahkan baris berikut di dalam kelas Account:

ii.	Modifikasi methode execute() dalam kelas Withdrawal untuk memeriksa apakah saldo setelah penarikan tidak kuran dari saldo minimal
 ![image](https://github.com/user-attachments/assets/4ce2df42-0fa8-417e-888f-677163bc34c6)
menambahkan logika dalam metode execute() di kelas Withdrawal untuk memeriksa apakah saldo setelah penarikan tidak kurang dari saldo minimal. Kelas Withdrawal harus mengimplementasikan metode execute() dan memverifikasi apakah penarikan tersebut bisa dilakukan berdasarkan saldo minimal yang ditentukan.

iii.	Jika saldo tidak mencukupi, tampilkan pesan kesalahan
![image](https://github.com/user-attachments/assets/705322a0-3041-469e-8442-36bf5bbc1a8c)
