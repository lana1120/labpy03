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
       - Program menghasilkan 5 angka random < 0,5 ;
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

   
