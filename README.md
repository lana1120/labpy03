# MODUL PRATIKUM 1

# LATIHAN 1

![CODINGAN 1](https://github.com/user-attachments/assets/c168472d-26ab-480c-8ef2-bf1639bf9cda)

Saya akan menjelaskan alur algoritma dari kode tersebut secara terstruktur :

1. **Insisialisasi**
   - Import fungsi random untuk menghasilkan angka acak
   - Meminta input niolai N dari user
   - Set counter awal = 1

2. **Proses utama ( Loop While )**
   ```
   WHILE Counter <=N
     1. Genrate angka random antara 0-1
     2. IF Angka random  < 0,5 :
        - Tampilkan "data ke -{counter} => {angka random}
        - Tambah counter dengan 1
     3. IF Angka random >= 0,5 :
        - Tidak melakukan apa apa
        - kembali ke langkah 1
    ```

3. **Kondisi terminasi**
    - Loop berhenti ketika counter > N
    - Tampilkan " SELESAI "

flowchart algoritma
```
Start
     ↓
    [Input nilai N]
    ↓
     [Set counter = 1]
    ↓
    ┌─────────────────────┐
    │ While counter <= N  │←──────┐
    └─────────┬───────────┘       │
              ↓                   │
        [Generate random]         │
              ↓                   │
        [Cek random < 0.5]        │
              ↓                   │
         [Jika Ya]──→[Print data] │
              ↓            ↓      │
         [Jika Tidak]   [counter++]
               │           │      │
               └───────────┘      │
                    ↑             │
                    └─────────────┘
                ↓
          [Print "Selesai"]
                ↓
               End
```

**Penjelasan detail**
1. program meminta user memasukan nilai N yang menentukan berapa banyak angka random < 0.5 yang di inginkan

2. program akan terus menghasilkan kata random samoai mendapatkan angka N buah angka yang nilainya < 0,5
   - jika angka random ≥ 0,5 : di abaikan dan generate angka baru
   - jika angka < 0,5 : di cetak dan counter bertambah

3. dari output yang terlihat
   - user masukan N = 5
   - Program menghasilkan 5 angka random < 0,5 :
```
       data ke: 1 => 0.22422725915012398
       data ke: 2 => 0.08143383880445236
       data ke: 3 => 0.29455614142741193
       data ke: 4 => 0.12537763804880175
       data ke: 5 => 0.46041201475820446
```

4. Setelah memndapatkan 5 angka yang memenuhi syarat, program selesai dan mencetak "Selesai"

Program ini mendemonstrasikan konsep:
 - Perulangan dengan kondisi (while loop)
 - Pengambilan keputusan (if condition)
 - Pembangkitan angka random
 - Pencacahan (counter)
 - Format string umtuk output

 - Saya akan menjelaskan alur algoritma dari kode perhitungan laba tersebut :

   # LATIHAN 2

   ![CODINGAN 2](https://github.com/user-attachments/assets/738793cb-3914-4b58-bad6-27159054de14)

1. **Inisialisasi**
   ```python
   laba_bulanan = []  # Array kosong untuk menyimpan laba per bulan
   total_laba = 0     # Variabel untuk menyimpan total laba
   modal_awal = 100000000  # Modal awal (tersirat dari output)
   

2. **Proses Perhitungan Laba (Loop pertama)**
   ```
   FOR bulan FROM 1 TO 8:
   
       1. Set laba = 0
       2. Hitung laba berdasarkan bulan:
          IF bulan <= 2:           # Bulan 1-2
             laba = 0
          ELSE IF bulan <= 4:      # Bulan 3-4
             laba = modal_awal * 1% (0.01)
          ELSE IF bulan <= 7:      # Bulan 5-7
             laba = modal_awal * 5% (0.05)
          ELSE:                    # Bulan 8
             laba = modal_awal * 2% (0.02)
       
       3. Simpan laba ke array laba_bulanan
       4. Tambahkan laba ke total_laba
   

4. **Proses Menampilkan Hasil (Loop kedua)**
   
   FOR bulan, laba IN laba_bulanan:
       Tampilkan "laba bulan ke-{bulan} sebesar: {laba}"
   
   Tampilkan "Total laba adalah: {total_laba}"
   

Flowchart algoritma:

             Start
               ↓
     [Inisialisasi variabel]
               ↓
     ┌─────────────────────┐
     │ For bulan 1 to 8    │
     └─────────┬───────────┘
               ↓
         [Set laba = 0]
               ↓
      [Cek kondisi bulan]
               ↓
       ┌─────────────────┐
       │ Bulan 1-2: 0%   │
       │ Bulan 3-4: 1%   │
       │ Bulan 5-7: 5%   │
       │ Bulan 8: 2%     │
       └────────┬────────┘
                ↓
          [Hitung laba]
                ↓
         [Simpan ke array]
                ↓
        [Update total_laba]
                ↓
       ┌─────────────────────┐
       │   For each laba     │
       └─────────┬───────────┘
                 ↓
       [Tampilkan laba per bulan]
                 ↓
         [Tampilkan total laba]
                 ↓
                End


**Output Program:** 

laba bulan ke- 1 sebesar: 0
laba bulan ke- 2 sebesar: 0
laba bulan ke- 3 sebesar: 1000000.0
laba bulan ke- 4 sebesar: 1000000.0
laba bulan ke- 5 sebesar: 5000000.0
laba bulan ke- 6 sebesar: 5000000.0
laba bulan ke- 7 sebesar: 5000000.0
laba bulan ke- 8 sebesar: 2000000.0
Total laba adalah: 19000000.0


*Penjelasan Logika Bisnis:*
1. Bulan 1-2: Belum ada laba (0%)
2. Bulan 3-4: Laba 1% dari modal
3. Bulan 5-7: Laba meningkat jadi 5% dari modal
4. Bulan 8: Laba turun menjadi 2% dari modal

Program ini mendemonstrasikan konsep:
- Array dan operasi append
- Perulangan (for loop)
- Pengambilan keputusan berjenjang (if-elif-else)
- Perhitungan persentase
- Akumulasi nilai
- Format string untuk output

 # LATIHAN 3

 ![CODINGAN 3](https://github.com/user-attachments/assets/8f27a26d-3e42-4d6f-a24a-b46e9b22b714)
  
1. **Inisialisasi Program**
```python
   def atm_simulator():
       saldo = 1000000  # Saldo awal
 ```  

2. **Alur Utama**
   
   LOOP Program ATM:

       1. Tampilkan menu:
          - 1. Tarik Uang
          - 2. Keluar
       2. Minta input pilihan menu (1/2)
       
       3. CASE Pilihan:
          CASE "1" (Tarik Uang):
             a. Minta input jumlah penarikan
             b. Validasi penarikan:
                IF jumlah > saldo:
                   Tampilkan "Maaf, saldo tidak mencukupi!"
                ELSE IF jumlah <= 0:
                   Tampilkan "Jumlah penarikan tidak valid!"
                ELSE:
                   Kurangi saldo dengan jumlah penarikan
                   Tampilkan "Penarikan berhasil!"
          
          CASE "2" (Keluar):
             a. Tampilkan "Terima kasih telah menggunakan ATM!"
             b. Keluar dari program (break)
          
          DEFAULT:
             Tampilkan "Pilihan tidak valid!"
   

**Flowchart algoritma :**

          Start
            ↓
    [Inisialisasi saldo]
            ↓
    ┌─────────────────────┐
    │ Loop ATM Program    │←──────────────────────────────┐
    └─────────┬───────────┘                               │
              ↓                                           │
       [Tampilkan Menu]                                   │
              ↓                                           │
        [Input Pilihan]                                   │
              ↓                                           │
          [Cek Pilihan]                                   │
              ↓                                           │
       ┌─────────────────┐                                │
       │ Pilihan = 1     │ ──→ [Input Jumlah]             |
       │ Pilihan = 2     │ ──→ [Tampil Terima Kasih]→[Exit]
       │ Pilihan Invalid │ ──→ [Tampil Error]             │
       └────────┬────────┘                                │
                ↓                                         │
        [Validasi Jumlah]                                 │
                ↓                                         │
          [Update Saldo]                                  │
                ↓                                         │
         [Tampil Status]                                  │
               └──────────────────────────────────────────┘


**Output Program yang terlihat :**
```
Saldo saat ini: Rp 1000000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 1
Masukkan jumlah penarikan: 730000
Penarikan berhasil!

Saldo saat ini: Rp 270000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 2
Terima kasih telah menggunakan ATM!
```

**Penjelasan Detail :**
1. **Struktur Data**
   - Variabel saldo: menyimpan saldo rekening
   - Variabel pilihan: menyimpan pilihan menu
   - Variabel jumlah: menyimpan jumlah penarikan

2. **Validasi**
   - Validasi pilihan menu (harus 1 atau 2)
   - Validasi jumlah penarikan:
     * Tidak boleh melebihi saldo
     * Tidak boleh negatif atau nol

3. **Fitur**
   - Cek saldo
   - Penarikan uang
   - Keluar dari program

Program ini mendemonstrasikan konsep:
- Function definition
- Loop control (break)
- Conditional statements (if-elif-else)
- Input/output handling
- Basic error handling
- Variable manipulation
- Menu-driven interface
