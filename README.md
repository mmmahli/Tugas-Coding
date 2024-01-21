# Tugas-Coding
Berisi tentang kumpulan tugas coding semasa TPB
# Code Program Kalkulator Sederhana
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
# Code Program Operasi Matriks
    #include <iostream>
    using namespace std;

    int main() {
        int baris, kolom, pilihan, det;
        char pilih;
        int matriks1[10][10], matriks2[10][10], hasil[10][10];
    
        do {
        cout << "====================================" << endl;
        cout << "PROGRAM KALKULATOR MATRIKS SEDERHANA" << endl;
        cout << "====================================" << endl;
        cout << "-Pilih Operasi Perhitungan-" << endl;
        cout << " 1. Pertambahan" << endl;
        cout << " 2. Pengurangan" << endl;
        cout << " 3. Transpose" << endl;
        cout << " 4. Perkalian matriks 2x2" << endl;
        cout << " 5. Determinan 2x2" << endl;
        cout << endl;
    
        cout << "Masukkan pilihan: ";
        cin >> pilihan;
        if (pilihan == 1){
            cout << "Masukkan jumlah baris: ";
            cin >> baris;
            cout << "Masukkan jumlah kolom: ";
            cin >> kolom;
        
            cout << "\nMasukkan elemen matriks pertama:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks1[i][j];
                }
            }
            cout << "\nMasukkan elemen matriks kedua:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks2[i][j];
                }
            }
            //Penjumlahan
            cout << "\nHasil penjumlahan matriks:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    hasil[i][j] = matriks1[i][j] + matriks2[i][j];
                    cout << hasil[i][j] << " ";
                }
                cout << endl;
            }
        }else if (pilihan == 2){
            cout << "Masukkan jumlah baris: ";
            cin >> baris;
            cout << "Masukkan jumlah kolom: ";
            cin >> kolom;
        
            cout << "\nMasukkan elemen matriks pertama:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks1[i][j];
                }
            }
            cout << "\nMasukkan elemen matriks kedua:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks2[i][j];
                }
            }
            //Pengurangan
            cout << "\nHasil pengurangan matriks:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    hasil[i][j] = matriks1[i][j] - matriks2[i][j];
                    cout << hasil[i][j] << " ";
                }
                cout << endl;
            }
        }else if (pilihan == 3){
            cout << "Masukkan jumlah baris: ";
            cin >> baris;
            cout << "Masukkan jumlah kolom: ";
            cin >> kolom;
        
            cout << "\nMasukkan elemen matriks :\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks1[i][j];
                }
            }
            //Transpose
            cout<<"hasil transpose matriks"<<endl;
              for(int i = 0; i < baris; i++){
                for(int j = 0; j < kolom; j++){
                   hasil[j][i] = matriks1[i][j] ;
                }
                cout << endl;
            }
        
              for(int i = 0; i<baris; i++){
                for(int j = 0; j < kolom;j++){
                    cout << hasil[i][j] << " ";
                }
                cout << endl;
            }
        }else if (pilihan == 4){
            cout << "Masukkan jumlah baris: ";
            cin >> baris;
            cout << "Masukkan jumlah kolom: ";
            cin >> kolom;
        
            cout << "\nMasukkan elemen matriks pertama:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks1[i][j];
                }
            }
            cout << "\nMasukkan elemen matriks kedua:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks2[i][j];
                }
            }
            //Perkalian
            cout << "\nHasil perkalian matriks:\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    hasil[i][j] = matriks1[i][j] * matriks2[i][j];
                    cout << hasil[i][j] << " ";
                }
                cout << endl;
            }
        }else if (pilihan == 5){
            cout << "Masukkan jumlah baris: ";
            cin >> baris;
            cout << "Masukkan jumlah kolom: ";
            cin >> kolom;
        
            cout << "\nMasukkan elemen matriks :\n";
            for (int i = 0; i < baris; i++) {
                for (int j = 0; j < kolom; j++) {
                    cin >> matriks1[i][j];
                }
            }
            //Determinan
            cout << "Hasil Determinan matriks" << endl;
              for(int i = 0; i < baris; i++){
                for(int j = 0; j < kolom; j++){
                   det = (matriks1[0][0] * matriks1[1][1]) - (matriks1[1][0] * matriks1[0][1]);
                }
            }
            cout << det << endl;
            } 
            
            cout << "Apakah anda ingin melakukan perhitungan lagi? (y/n): ";
            cin >> pilih;
            system("clear");
        } while (pilih == 'y' || pilih == 'Y');
        
        return 0;
    }
# Code Program Persegi #O
    #include <iostream>
    using namespace std;
    
    int main() {
        int N, i, j;
        
        cout << "Masukkan sebuah bilangan bulat: ";
        cin >> N;
        
        
        for (i = 1; i <= N; i++) {
            for (j = 1; j <= N; j++){
                if (i%2 != 0 && j%2 != 0 || i%2 == 0 && j%2 == 0) {
                    cout << "#";
                }else {
                    cout << "O";
                }
            }
            cout << endl;
        }
        return 0;
    }
# Code Program Persegi Bolong
    #include <iostream>
    using namespace std;
    
    int main() {
        int N, i, j;
        
        cout << "masukkan nilai N: ";
        cin >> N;
        
        for (i = 1; i <= N; i++) {
            for (j = 1; j <= N; j++) {
                if (i == 1 || i == N || j == 1 || j == N) {
                    cout << "#";
                }else {
                    cout << " ";
                }
                
            }
            cout << endl;
        }
        return 0;
    }
# Code Program Bilangan Positif Negatif
    #include<iostream>
    using namespace std;
    
    int main(){
        int bilangan;
        string tanda;
        
        cout<<"================================"<<endl;
        cout<<"Program Positif, Negatif dan Nol"<<endl;
        cout<<"================================"<<endl;
        cout<<" "<<endl;
        cout<<"Masukkan Bilangan = ";
        cin>>bilangan;
        
        if(bilangan > 0){
            tanda = "Positif";
        }else if(bilangan < 0){
            tanda = "Negatif";
        }else if(bilangan == 0){
            tanda = "Nol";
        }
        
        cout<<"Bilangan "<<bilangan<<" adalah bilangan = "<<tanda;
    }
# Code Program  Rata-Rata Nilai
    #include <iostream>
    using namespace std;
    int main(){
    	float a,b,c,d,e,f;
    	string g,h,i,j,k;
    	cout<<"Masukkan nama mahasiswa pertama: ";
    	cin>>g;
    	cout<<"Masukkan nilai "<<g<<" : ";
    	cin>>a;
    	cout<<"Masukkan nama mahasiswa kedua: ";
    	cin>>h;
    	cout<<"Masukkan nilai "<<h<<" : ";
    	cin>>b;
    	cout<<"Masukkan nama mahasiswa ketiga: ";
    	cin>>i;
    	cout<<"Masukkan nilai "<<i<<" : ";
    	cin>>c;
    	cout<<"Masukkan nama mahasiswa keempat: ";
    	cin>>j;
    	cout<<"Masukkan nilai "<<j<<" : ";
    	cin>>d;
    	cout<<"Masukkan nama mahasiswa kelima: ";
    	cin>>k;
    	cout<<"Masukkan nilai "<<k<<" : ";
    	cin>>e;
    	f=(a+b+c+d+e)/5;
    	cout<<"Rata rata nilai: "<<f;
    	
    }
# Code Program Segitiga Rata Kanan Menurun
    #include <iostream>
    using namespace std;
    
    int main() {
        int i, n, j, k;
        
        cout << "Masukkan nilai n: ";
        cin >> n;
        
        
        for (i = 1; i <= n; i++) {
            for (j = 1; j <= n - i; j++) {
                cout << " ";
            }
            for (k = 1; k <= i; k++) {
                cout << n--;
            }
            n += i;
            cout << endl;
        }
        return 0;
    }    
# Code Program Luas Keliling Trapesium
    #include <iostream>
    using namespace std;
    int main(){
    	float a,b,c,d,e,f;
    	cout<<"Masukkan panjang sisi atas: ";
    	cin>>a;
    	cout<<"Masukkan panjang sisi bawah: ";
    	cin>>b;
    	cout<<"Masukkan panjang sisi samping: ";
    	cin>>c;
    	cout<<"Masukkan tinggi: ";
    	cin>>d;
    	e=(d*(a+b)/2);
    	f=a+b+c+d;
    	cout<<"Luas trapesium: "<<e<<endl;
    	cout<<"Keliling trapesium: "<<f<<endl;
    }
# Code Program Nilai Sama Maka Mengulang
    #include <iostream>
    using namespace std;
    
    int main() {
        int a, b, c;
    
        do{
           cout << "Masukkan nilai a = "  ;
           cin >> a ;
           cout << "Masukkan nilai b = "  ;
           cin >> b ;
           cout << "Masukkan nilai c = "  ; 
           cin >> c ;
        }while (a==b||a==c||b==c) ;
        
        return 0;
    }    
# Code Program Nilai Faktorial
    #include <iostream>
    using namespace std;
    
    int main() {
        int i, n, hasil;
        
        cout << "Masukkan angka: ";
        cin >> n;
        
        hasil = 1;
        for (i = 1; i <= n; i++) {
            hasil = hasil * i;
        }
        cout << "Nilai faktorial dari " << n << " adalah " << hasil;
        
        return 0;
    }
# Code Program Perhitungan
    #include <iostream>
    using namespace std;
    int main(){
    	
    	float a,b;
    	cout<<"Masukkan nilai pertama: ";
    	cin>>a;
    	cout<<"Masukkan nilai kedua: ";
    	cin>>b;
    	
    	cout<<"Hasil dari pertambahan: " <<a<< " + " <<b<< " = " <<a + b <<endl;
    	cout<<"Hasil dari pengurangan: " <<a<< " - " <<b<< " = " <<a - b <<endl;
    	cout<<"Hasil dari pembagian: " <<a<< " / " <<b<< " = " <<a / b <<endl;
    	cout<<"Hasil dari perkalian: " <<a<< " * " <<b<< " = " <<a * b <<endl;
    	cout<<"Hasil dari modulus: " <<a<< " % " <<b<< " = " <<(a/b)*b;

        return 0;
    }
# Code Program Hitung Nilai Akhir Mata Kuliah
    #include <iostream>
    using namespace std;
    
    int main(){
    	string Nama,Matkul;
    	float Tugas,UTS,UAS,Nilai;
    	
    	cout<<"Program Hitung Nilai Akhir Mata Kuliah" <<endl;
    	cout<<"Masukkan nama mahasiswa: ";
    	cin>>Nama;
    	cout<<"Masukkan nama matkul " <<Nama<< ": ";
    	cin>>Matkul;
    	cout<<"Masukkan nilai tugas " <<Matkul<< ": ";
    	cin>>Tugas;
    	cout<<"Masukkan nilai UTS " <<Matkul<< ": ";
    	cin>>UTS;
    	cout<<"Masukkan nilai UAS " <<Matkul<< ": ";
    	cin>>UAS;
    	Nilai=(0.4*Tugas) + (0.3*UTS) + (0.3*UAS);
    	cout<< "Nilai akhir " <<Matkul<< " " <<Nama<< ": " <<Nilai;
     
    	return 0;
    }
# Code Program Menentukan Bulan Dengan Angka
    #include <iostream>
    using namespace std;
    
    int main() {
      int n;
      string bulan;
    
      cin >> n;
      if(n==1){
          bulan = "januari";
      }else if(n==2){
          bulan = "februari";
      }
      else if(n==3){
          bulan = "maret";
      }
      else if(n==4){
          bulan = "april";
      }
      else if(n==5){
          bulan = "mei";
      }
      else if(n==6){
          bulan = "juni";
      }
      else if(n==7){
          bulan = "juli";
      }
      else if(n==8){
          bulan = "agustus";
      }
      else if(n==9){
          bulan = "september";
      }
      else if(n==10){
          bulan = "oktober";
      }
      else if(n==11){
          bulan = "november";
      }else if(n==12){
          bulan = "desember";
      }else{
          bulan = "Salah, Masukkan antara 1-12";
      }
      cout << bulan << endl;
    
      return 0;
    }
