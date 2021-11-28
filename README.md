# Labspy04
## Latihan List

### Akses List
- Tampilkan elemen ke-3
- Ambil nilai elemen ke-2 sampai elemen ke-4
- Ambil elemen terakhir

#### Program
![Gambar1](Ss/1.jpeg)
#### Penjelasan
1. Membuat list dengan nilai yang diinginkan
```python
bungan = ['mawar', 'melati', 'tulip', 'kamboja', 'laveder', 'teratai']
```
2. Menampilakn semua elemen yang terdapat pada list diatas
```python
print("bunga :", bunga)
3. Untuk menampilkan salah satu element dalam sebuah list dapat menggunakan `bunga[2]`
```python
print('Elemen ke-3', bunga[2])
```
4. Jika ingin mengambil elemen ke-2 sampai elemen ke-4 dapat menggunakan `bunga[1:5]`
```python
print('Elemen ke-2 sampai ke-4', bunga[1:5])
```
5. Jika ingin mengambil elemen terakhir dapat menggunakan `bunga[-1]`
```python
print ('Elemen terakhir', bunga[-1])
```
#### Output
![Gambar2](Ss/2.jpeg)
### Mengubah Elemen List
- Ubah elemen ke-4 dengan nilai lainnya
- Ubah elemen ke-4 sampai dengan elemen terakhir

#### Program
![Gambar3](Ss/3.jpeg)
#### Penjelasan
1. Membuat list dengan nilai yang diinginkan
```python
bunga = ['mawar', 'melati', 'tulip', 'kamboja', 'levender', 'teratai']
 2. Menampilakn semua elemen yang terdapat pada list diatas
```python
bunga[3] = 'kembang sepatu'
print("bunga sesudah di ubah:", bunga)
```
3. Jika ingin mengubah elemen ke-4 sampai dengan elemen terakhir dapat menggunakan `bunga[3:]`
```python
bunga[3:] = ["matahari", "calla lily"]
print("ubah elemen ke-4 hingga akhir :", bunga)
```
### Output
![Gambar4](Ss/4.jpeg)
### Menambahkan Elemen List
- Ambil 2 bagian dari list pertama (A) dan jadikan list ke-2 (B)
- Tambah list B dengan nilai string
- Tambah list B dengan 3 nilai
- Gabungkan list B dengan list A

#### Program
![Gambar5](Ss/5.jpeg)
#### Penjelasan
1. Membuat list dengan variabel a dan b
```python
a = [6, 7, 8, 9, 10]
b = [11, 12, 13, 14, 15]
```
2. Untuk mengambil 2 bagian dari list a dan dijadikan list b
```python
b.append(a[0:2])
print(b)
```

3. Untuk menambahkan list b dengan nilai string 
```python
b.append("13")
print(b)
```
4. Untuk menambahkan list b dengan 3 nilai
```python
print()
print(b + [12, 13, 14])
```

5. Untuk menggabungkan list b dengan list a
```python
print()
print(a + b)
```
#### Output
![Gambar6](Ss/6.jpeg)

## Tugas Praktikum
### Program sederhana untuk menambahkan data kedalam sebuat list 
#### Program
![Gambar7](Ss/flowchart.jpeg)
![Gambar8](Ss/7.png)
#### Penjelasan
1. Mendeklarasi list
```python
_nama = []
_nim = []
_tugas = []
_uts = []
_uas = []
_akhir = []
```

2. Gunakan perulangan _while loop_ dengan nilai "True"
```python
while True:
```

3. Menginput nama, nim, tugas, uts, uas, dan akhir dengan menambahkan method `.append`
```python
 _nama.append(input("Masukan nama : "))
    _nim.append(input("Masukan NIM  : "))
    tugas = int(input("Nilai tugas  : ")); _tugas.append(tugas)
    uts   = int(input("Nilai UTS    : ")); _uts.append(uts)
    uas   = int(input("Nilai UAS    : ")); _uas.append(uas)

    _akhir.append(tugas * 30/100 + uts * 35/100 + uas * 35/100)
```

4. Pada input <b>Tambah Data Lagi?</b> apabila jawaban “t” atau “T”, maka program akan berhenti dan akan menampilkan hasil daftar datanya
```python
_tanya = input("Tambah data lagi? [y/t]: ")
    print()
    if(_tanya == "t" or _tanya =="T"):
        break
```

5. Untuk membuat header table, menggunakan `print(73*"=")`, fungsinya membuat "=" sebanyak 73 sebagai garis, dan menggunakan format string
```python
print(73*"=")
print("| {0:^2} | {1:^18} | {2:^9} | {3:^5} | {4:^5} | {5:^5} | {6:^7} |".format("No", "Nama", "NIM", "Tugas", "UTS", "UAS", "Akhir"))
print(73*"=")
```

6. Deklarasi `no = 0` untuk membuat nomor pada isi table, lalu membuat perulangan dengan `for`
- Perulangan `nama, nim, tugas, uts, uas`, sesuai urutan yang ada di dalam `zip`
- Pada list yang dimaksud, `in zip` berfungsi untuk membungkus semua list
```python
no = 0
for nama, nim, tugas, uts, uas, akhir in zip(_nama, _nim, _tugas, _uts, _uas, _akhir):
```

7. Membuat isi tabel sesuai keinginan dengan format string
```python
no += 1    
    print("| {0:>2} | {1:<18} | {2:>9} | {3:>5} | {4:>5} | {5:>5} | {6:>7.2f} |".format(no, nama, nim, tugas, uts, uas, akhir))
```

8. Untuk membuat footer atau garis paling bawa ketika looping isi table selesai
```python
print(73*"=")
```
#### Output
![Gambar9](Ss/8.png)

#### Selesai


