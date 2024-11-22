Nama  : Moh. Raihan Al Fikrii
Nim   : 352310871
Kelas : IE.23.C12

# Program untuk menambahkan data ke dalam list

# List untuk menyimpan data mahasiswa
data_mahasiswa = []

while True:
    # Memasukkan data mahasiswa
    nama = input("Nama: ")
    nim = input("NIM: ")
    nilai_tugas = float(input("Nilai Tugas: "))
    nilai_uts = float(input("Nilai UTS: "))
    nilai_uas = float(input("Nilai UAS: "))
    
    # Menghitung nilai akhir
    nilai_akhir = (nilai_tugas * 0.3) + (nilai_uts * 0.35) + (nilai_uas * 0.35)
    
    # Menambahkan data ke dalam list
    data_mahasiswa.append({
        "Nama": nama,
        "NIM": nim,
        "Tugas": nilai_tugas,
        "UTS": nilai_uts,
        "UAS": nilai_uas,
        "Akhir": nilai_akhir
    })
    
    # Menanyakan apakah ingin menambahkan data lagi
    tambah_data = input("Tambah data (y/t)? ").lower()
    if tambah_data == 't':
    ![Screenshot 2024-11-23 023912](https://github.com/user-attachments/assets/d200ca67-693c-4ef8-adb9-033f6372fef5)
    ![Flowchart proses](https://github.com/user-attachments/assets/e602d3c9-40de-402f-ba24-1bbce0f00ddb)


        break

# Menampilkan data
print("\n{:<5} {:<15} {:<10} {:<10} {:<10} {:<10} {:<10}".format(
    "No", "Nama", "NIM", "Tugas", "UTS", "UAS", "Akhir"))
print("=" * 65)

for i, mahasiswa in enumerate(data_mahasiswa, start=1):
    print("{:<5} {:<15} {:<10} {:<10} {:<10} {:<10} {:<10.2f}".format(
        i, mahasiswa["Nama"], mahasiswa["NIM"], mahasiswa["Tugas"],
        mahasiswa["UTS"], mahasiswa["UAS"], mahasiswa["Akhir"]))
![Screenshot 2024-11-23 023912](https://github.com/user-attachments/assets/f6c8b436-2ee7-4ab5-a51c-453099bec8b6)

Penjelasan :

List data_nilai: Digunakan untuk menyimpan data yang dimasukkan, termasuk nilai tugas, UTS, UAS, dan nilai akhir.
Perulangan while True: Perulangan yang terus berlangsung selama pengguna memilih untuk menambah data (menjawab "y").
Input Nilai: Program meminta input nilai tugas, UTS, dan UAS, kemudian menghitung nilai akhir berdasarkan bobot yang diberikan.
Menyimpan Data: Data dimasukkan ke dalam list data_nilai, di mana setiap elemen berupa list yang berisi nilai tugas, UTS, UAS, dan nilai akhir.
Pertanyaan untuk Menambah Data: Setelah memasukkan data, program akan menanyakan apakah ingin menambah data lagi dengan menjawab "y" (ya) atau "t" (tidak).
Menampilkan Daftar Nilai: Jika pengguna memilih untuk tidak menambah data, program akan menampilkan seluruh data yang telah dimasukkan dengan format yang rapi

FLOW CHART

![Flowchart proses](https://github.com/user-attachments/assets/1f40bb62-2faa-420b-93a6-164894b70e1f)



        
        
