### Nama  : Esa Alliant.
### Absen : 24.
### kelas : XII Rpl 1

# modul 4.
# VIEW BLADE TEMPLATE
-->View merupakan bagian yang menampilkan informasi untuk disampaikan kepada users. View 
terdiri dari script HTML dengan bantuan CSS dan javascript. Sesuai dengan aturan konsep MVC, di 
dalam view tidak boleh ada script logika maupun script untuk mengakses database. Di dalam laravel 
view diletekan di dalam folder resources/views/. 

kita buat file 
```php artisan make:controller BarangController```
lalu click program ini 
```public function index()
    {
        return view ('kategori.kategori');
    }
```
ini gambar nya 

![image](https://user-images.githubusercontent.com/109930667/183345033-e0f8e209-741e-413d-bae0-baea38f5ac06.png)

kemudian pilih file web{

![image](https://user-images.githubusercontent.com/109930667/183345173-a9e3e604-1ac7-4efc-bcc4-5437d3145c25.png)

Habis itu ketik program di bawah.

![image](https://user-images.githubusercontent.com/109930667/183350244-054445f8-d1bd-4f28-913a-31d3a889ac33.png)

 jangan lupa di sama di atas nya di ketik program ini . supaya tidak terjadi error.

![image](https://user-images.githubusercontent.com/109930667/183350540-5ea08b05-3f86-4047-b069-690a541a38fd.png)

jika kalian menjalan kan program hasil nya seperti ini.

![image](https://user-images.githubusercontent.com/109930667/183352193-c8789a66-9a17-4b38-a69e-665bf2ec0ac8.png)

TUGAS PRAKTIKUM
1. Buatlah View untuk project anda
2. Buatlah layout dengan master template blade untuk project anda.
___________________________________________________________________________________________________________________________________________________________________
#TUGAS PRAKTIKUM
### 1. buatlah view untuk project anda.
Langkah 1.
pertama cari resources.lalu pilih view.

![image](https://user-images.githubusercontent.com/109930667/183354183-ba185a10-9826-4a04-8464-0176035f72d2.png)

klick kiri pada view.sesudah milih pakai nama *barang*.lalu klick lagi terus membuat file contoh nomer 2 pada gambar+ hasil.

![image](https://user-images.githubusercontent.com/109930667/183355115-ea8ef4d6-20e0-4cd9-bebb-8a12c7a6890b.png)

### 2. Buatlah layout dengan master template blade untuk project anda.

tulis program di bawah ini.

```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css">
    <title>
        @yield('tiitle')
    </title>
</head>
<body>

    <div class= "container">
        <nav class="navbar navbar-expand-lg bg-dark">
            <div class="container-fluid">
              <a class="navbar-brand text-light" href="#">penjualan</a>
              <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                  <li class="nav-item">
                    <a class="nav-link active text-light" aria-current="page" href="/">Home</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link text-light" href="/barang">barang</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link text-light" href="/kategori">kategori</a>
                  </li>
              </div>
            </div>
          </nav>
    </div>

    <div class="container">
        @yield('content')
    </div>
    
    <script> scr="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.j"</script>
</body>
</html>
```

ini hasil program.
![image](https://user-images.githubusercontent.com/109930667/183356328-85b3806b-cebe-4726-b832-9c76b4d73638.png)






