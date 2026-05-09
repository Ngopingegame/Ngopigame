<!DOCTYPE html>
<html>
<head>
   <title>ngopingegame</title>
</head>
<body>

<h1>SELAMAT DATANG</h1>
<p>Website DI WARUNG KAMI </p>

</body>
</html>

nama = input("Nama pelanggan: ")

jam = int(input("Berapa jam main: "))

# Tarif PS
if jam >= 3:
    harga_per_jam = 5000
else:
    harga_per_jam = 6000

total_ps = jam * harga_per_jam

total_makanan = 0

lagi = "y"

while lagi == "y":

    print("===== MENU =====")
    print("1. Mie Rebus = 6000")
    print("2. Kopi Hitam = 3000")
    print("3. Teh Hangat = 3000")
    print("4. Es Teh = 4000")
    print("5. Es Nutrisari = 4000")
    print("6. Es Susu = 5000")
    print("7. Good Day Freeze = 5000")

    pilihan = int(input("Pilih menu: "))

    if pilihan == 1:
        total_makanan += 6000
    elif pilihan == 2:
        total_makanan += 3000
    elif pilihan == 3:
        total_makanan += 3000
    elif pilihan == 4:
        total_makanan += 4000
    elif pilihan == 5:
        total_makanan += 4000
    elif pilihan == 6:
        total_makanan += 5000
    elif pilihan == 7:
        total_makanan += 5000

    lagi = input("Tambah menu lagi? (y/t): ")

# Total akhir
total = total_ps + total_makanan

print("==========")
print("Pelanggan :", nama)
print("Biaya PS :", total_ps)
print("Makanan/Minuman :", total_makanan)
print("Total bayar :", total)
print("==========")
