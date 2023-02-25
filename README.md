# game1
Predict the number

import random

def main():
    # Menentukan angka acak antara 1 dan 100
    number = random.randint(1, 100)

    print("Selamat datang di Tebak Angka!")
    print("Saya telah memilih angka antara 1 dan 100.")
    print("Silakan tebak angka tersebut.")

    # Menerima input dari pemain
    guess = int(input("Tebakan Anda: "))

    # Membandingkan tebakan dengan angka acak
    while guess != number:
        if guess < number:
            print("Terlalu rendah. Silakan coba lagi.")
        else:
            print("Terlalu tinggi. Silakan coba lagi.")

        guess = int(input("Tebakan Anda: "))

    # Jika tebakan benar, cetak pesan kemenangan
    print("Selamat! Anda berhasil menebak angka saya.")

if __name__ == '__main__':
    main()
