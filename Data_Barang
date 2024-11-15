# data_barang.py

# Daftar barang sembako yang tersedia di toko
data_barang = [
    {"kode": "BRG001", "nama": "Beras", "stok": 100, "harga": 12000},
    {"kode": "BRG002", "nama": "Gula", "stok": 50, "harga": 14000},
    {"kode": "BRG003", "nama": "Minyak Goreng", "stok": 30, "harga": 18000},
    {"kode": "BRG004", "nama": "Tepung Terigu", "stok": 75, "harga": 10000},
    {"kode": "BRG005", "nama": "Garam", "stok": 200, "harga": 5000},
    # Tambahkan barang hingga mencapai 50 data
    # ...
]

# Fungsi untuk menampilkan daftar barang
def tampilkan_data_barang():
    print("\nData Barang Toko Sembako\n")
    print("Kode\tNama Barang\tStok\tHarga")
    print("-" * 40)
    for barang in data_barang:
        print(f"{barang['kode']}\t{barang['nama']}\t{barang['stok']}\t{barang['harga']}")
    print("-" * 40)

# Fungsi untuk menambah barang baru
def tambah_barang():
    kode = input("Masukkan kode barang: ")
    nama = input("Masukkan nama barang: ")
    stok = int(input("Masukkan jumlah stok: "))
    harga = int(input("Masukkan harga barang: "))

    # Tambah data barang ke dalam list data_barang
    data_barang.append({"kode": kode, "nama": nama, "stok": stok, "harga": harga})
    print(f"Barang {nama} berhasil ditambahkan.")

# Fungsi untuk menghapus barang
def hapus_barang():
    kode = input("Masukkan kode barang yang akan dihapus: ")
    barang_ditemukan = False

    # Cari dan hapus barang berdasarkan kode
    for barang in data_barang:
        if barang["kode"] == kode:
            data_barang.remove(barang)
            print(f"Barang dengan kode {kode} berhasil dihapus.")
            barang_ditemukan = True
            break

    if not barang_ditemukan:
        print(f"Barang dengan kode {kode} tidak ditemukan.")

# Fungsi untuk mencari barang berdasarkan kode
def cari_barang():
    kode = input("Masukkan kode barang yang ingin dicari: ")
    barang_ditemukan = False

    for barang in data_barang:
        if barang["kode"] == kode:
            print("\nData Barang")
            print("Kode\tNama Barang\tStok\tHarga")
            print(f"{barang['kode']}\t{barang['nama']}\t{barang['stok']}\t{barang['harga']}")
            barang_ditemukan = True
            break

    if not barang_ditemukan:
        print(f"Barang dengan kode {kode} tidak ditemukan.")

# Fungsi utama untuk menampilkan menu
def main():
    while True:
        print("\nMenu Toko Sembako")
        print("1. Tampilkan Daftar Barang")
        print("2. Tambah Barang Baru")
        print("3. Hapus Barang")
        print("4. Cari Barang")
        print("5. Keluar")
        pilihan = input("Pilih menu: ")

        if pilihan == "1":
            tampilkan_data_barang()
        elif pilihan == "2":
            tambah_barang()
        elif pilihan == "3":
            hapus_barang()
        elif pilihan == "4":
            cari_barang()
        elif pilihan == "5":
            print("Keluar dari program.")
            break
        else:
            print("Pilihan tidak valid, silakan coba lagi.")

# Jalankan fungsi utama
if __name__ == "__main__":
    main()
