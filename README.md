# Tugas-Coding
Berisi tentang kumpulan tugas coding semasa TPB
# Code Kalkulator sederhana
    //Muhammad Ilham_122130031_Teknik Elektro
    //Tugas 3 Self Solving

    #include <iostream>
    using namespace std;

    int main() {
      char pilihan;
      float angka1, angka2;
    
     do {
        cout << "===========================" << endl;
        cout << "PROGRAM KALKULATOR SEDRHANA" << endl;
        cout << "===========================" << endl;
        cout << "-Pilih Operasi Perhitungan-" << endl;
        cout << " 1. Penjumlahan" << endl;
        cout << " 2. Pengurangan" << endl;
        cout << " 3. Perkalian" << endl;
        cout << " 4. Pembagian" << endl;
        cout << " 5. Modulus" << endl;

        cout << "Masukkan pilihan anda (1-5): ";
        cin >> pilihan;

        cout << "Masukkan angka pertama: ";
        cin >> angka1;
        cout << "Masukkan angka kedua: ";
        cin >> angka2;

        switch (pilihan) {
            case '1':
                cout << " Hasil dari penjumlahannya = " << angka1 + angka2 << endl;
                break;
            case '2':
                cout << " Hasil dari pengurangannya = " << angka1 - angka2 << endl;
                break;
            case '3':
                cout << "Hasil dari perkaliannya = " << angka1 * angka2 << endl;
                break;
            case '4':
                cout << "Hasil dari pembagiannya = " << angka1 / angka2 << endl;
                break;
            case '5':
                cout << "Hasil dari modulusnya = " << angka1 - ((angka1 / angka2) * angka2) << endl;
                break;
            default:
                cout << "Angka yang anda masukkan salah. Silahkan coba lagi." << endl;
        }

        cout << "Apakah Anda ingin melakukan perhitungan lagi? (y/n): ";
        cin >> pilihan;
        
    } while (pilihan == 'y' || pilihan == 'Y');

    return 0;
    }
