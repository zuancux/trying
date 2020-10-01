# Tutorial APAP
## Authors
* **Vikih Fitrianih** - *1806191130* - *D*


#Tutorial 2



**Pertanyaan 1: Cobalah untuk menambahkan sebuah resep dengan mengakses link berikut:**
http://localhost:8080/resep/add?noResep=1&namaDokter=Papa%20APAP&namaPasien=Quanta%20Fasilkom&catatan=Semangat 
**Apa yang terjadi? Jelaskan mengapa hal tersebut dapat terjadi**

**jawab :**
Terjadi erorr, karena template add-resep belum ada, sedangkan input parameter di render ke add-resep(template belum ada). 

![nomor 1](https://github.com/zuancux/trying/blob/master/pertanyaan%201.png)


**Pertanyaan 2: Menurut kamu anotasi @Autowired pada class Controller tersebut merupakan implementasi dari konsep apa? Dan jelaskan secara singkat cara kerja @Autowired tersebut dalam konteks service dan controller yang telah kamu buat**

@Autowired pada class Controller tersebut merupakan implementasi dari konsep DI Spring. @Autowired akan melakukan component-scan, yaitu dia akan melihat isi package yang kita sebutkan, kemudian akan mencari class-class yang diberi anotasi berikut:
@Repository, @Service, @Controller dan @Component
Setelah ditemukan, maka dia akan melakukan inisialisasi terhadap class ResepService dan ResepController, dan lalu mengisi (inject) semua kebutuhannya (dependency). 




**Pertanyaan 3: Cobalah untuk menambahkan sebuah resep dengan mengakses link berikut:** http://localhost:8080/resep/add?noResep=1&namaDokter=Papa%20APAP&namaPasien=Quanta%20Fasilkom 
**Apa yang terjadi? Jelaskan mengapa hal tersebut dapat terjadi.**

**jawab :**
Error, tidak ada parameter catatan, padahal diminta argumen catatan
![nomor 3] (https://drive.google.com/file/d/1PR0BAWJ2fARYXrMLSeB2216QRM4Tcgit/view?usp=sharing)

**Pertanyaan 4: Jika Papa APAP ingin melihat resep untuk pasien yang bernama Quanta, link apa yang harus diakses?**
**jawab : **
http://localhost:8080/resep/view?noResep=1

![nomor 4](https://drive.google.com/file/d/1S7hHKj5bbC7JIshYGBO8s0TUu5-5guCu/view?usp=sharing)

**Pertanyaan 5: Tambahkan 1 contoh resep lainnya sesukamu. Lalu cobalah untuk mengakses** http://localhost:8080/resep/viewall **, apa yang akan ditampilkan? Sertakan juga bukti screenshotmu**
**jawab :**
Menampilkan seluruh daftar resep
![nomor 5] (https://drive.google.com/file/d/1KCGj0LD0bgLFpeDRbr6aYBtlPGWvJu0n/view?usp=sharing)
