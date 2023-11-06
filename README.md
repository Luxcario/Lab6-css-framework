# Lab6-css-framework

# Membuat Layout sederhana

# Membuat Struktur dasar Html
Struktur dasar Html terdiri dari ```html``` ```head``` ```title``` ```body``` agar lebih mudah ketik ```!``` lalu enter, seperti berikut
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

# Import Bundle Bootstrap CSS
copy kode pada website bootsrap http://getbootstrap.com/ , masukkan Reference didalam head agar dapat menggunakan Twitter Bootstrap
```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
```


# Membuat Navigasi
buat div untuk bungkusan, gunakan Header untuk judul utama pada layout masukkan tag ```<h1>``` untuk membuat nama judul, setelah itu buat tag ```<nav>``` untuk navigasi beserta tag ```<a>``` ditambah atribut href unutk referensi pada pilihan navigasi
```
<div>
  <header>
    <h1>Layout Sederhana</h1>
  </header>
  <nav>
    <a href="#" class="active">Home</a>
    <a href="#article">Artikel</a>
    <a href="#about">About</a>
    <a href="#contact">Kontak</a>
  </nav>
</div>
```

# Membuat Dokumen
gunakan ```<section>``` untuk membuat dokumen ditambah tag id untuk membuat style nanti,```<section>``` wajib menggunakan judul maka buat judul menggunakan tag ```<h2>``` atau yang lain, buat isi dokumen berupa paragrah menggunakan tag```<p>```
```
<section id="hero">
  <h2>Hello World!</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
  elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
  vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
  pretium ac.</p>
</section>
```
**Run untuk melihat hasil**

![image](https://github.com/Luxcario/Lab6-css-framework/assets/116184002/adc6bf3c-1229-43cc-b88d-77a87062c9e6)

# Membuat content
buat bungkusan keseluruhan content menggunakan ```div``` dan tambahkan atribut ```id``` beri nama apasaja, tambahkan ```section``` sebagain dokumen dan tambahkan ```id```nya, buat ```div``` lagi untuk bungkusan dari luaran isi content, dan bungkusan untuk content, gunakan tag ```<img>``` untuk memasukkan gambar di dalam dokumen dan tambahkan atribut ```src``` untuk memanggil gambar pada folder ke dalam dokumen, masukkan saja ```alt``` sebagai syarat dari penggunaan ```<img>```, buat class untuk mengatur gambar, tambahkan judul content menggunakan ```h3```, lalu tambahkan paragraf menggunakan tag```p``` dan paragrafnya, tambahkan ```a```, ```href``` dan ```class```, agar terkoneksi dengan navigasi. buat 3 content
```
<div id="wrapper">
<section id="main">
  <div class="row">
    <div class="box">
      <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
      <h3>Heading</h3>
      <p>Donec sed odio dui. Etiam porta sem malesuada magna molliseuismod.</p>
      <a href="#" class="btn btn-default">View detail</a>
    </div>
    <div class="box">
      <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
      <h3>Heading</h3>
      <p>Donec sed odio dui. Etiam porta sem malesuada magna molliseuismod.</p>
      <a href="#" class="btn btn-default">View detail</a>
    </div>
    <div class="box">
      <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
      <h3>Heading</h3>
      <p>Donec sed odio dui. Etiam porta sem malesuada magna molliseuismod.</p>
      <a href="#" class="btn btn-default">View detail</a>
    </div>
  </div>
  <hr class="divider" />
</section>
</div>
```
tambahkan ```<hr>``` untuk membuat garis batas content

# Membuat Article
Gunakan tag ```article``` untuk membuat artikel, buat class dan idnya, dan gunakan tag-tag untuk memasukkan gambar, paragraf dan lain lain
```
<article class="entry" id="article">
  <h2>First featurette heading.</h2>
  <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,vestibulum mi porta, faucibus felis. Integer
pharetra est nunc, nec pretium nuncpretium ac.</p>
</article>
  <hr class="divider" >
  <article class="entry">
  <h2>First featurette heading.</h2>
  <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum loremelit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nuncpretium ac.</p>
</article>
```

# Membuat Sidebar
untuk membuat sidebar gunakan tag ```aside``` dan tambahkan idnya, buat bungkusan menggunakan ```div``` dan tambahkan class, gunakan tag ```<li>``` untuk membuat list secara tidak terurut masukkan ```<a>``` dan tambahkan ```href``` untuk referensi link yang akan dibuat.
```
<aside id="sidebar">
  <div class="widget-box">
    <h3 class="title">Widget Header</h3>
      <ul>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
        <li><a href="#">Widget Link</a></li>
      </ul>
  </div>
  <div class="widget-box">
    <h3 class="title">Widget Text</h3>
      <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tinciduntarcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integerpharetra est nunc, nec pretium nunc pretium ac.</p>
  </div>
</aside>
```

**Run untuk melihat Hasilnya**

![image](https://github.com/Luxcario/Lab6-css-framework/assets/116184002/f0bcbf0a-5a65-4646-a6d0-6171da8d97a4)

![image](https://github.com/Luxcario/Lab6-css-framework/assets/116184002/41ed4deb-9412-4fce-80e1-95a5e29a4aa1)

# Membuat Footer
gunakan tag ```footer``` untuk membuat footer, dan masukkan footer berupa paragraf/teks, tanda ```&copy``` untuk membuat lambang C.
```
<footer>
  <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```
**hasil Run**

![image](https://github.com/Luxcario/Lab6-css-framework/assets/116184002/51ee8a58-b0b1-4167-9cea-53a27a0a14c2)

# Membuat style menggunakan CSS Internal
Masukkan Kode seperti berikut pada bagian ```<head>```
```
<style>
        *{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: "Open Sans", sans-serif;
            font-size: 100%;
        }

        #container {
            height: 1300px;
        }

        nav a.active,
        nav a:hover {
            background-color: #68a4e8;
        }

        .widget-box li:hover a {
            background-color: #eee;
        }

        .row:after,
        .row:before,
        .entry:after,
        .entry:before {
            content: "";
            display: table;
        }

        .row:after,
        .entry:after {
            clear: both;
        }
    </style>
```

# Menambahkan Twiter Bootstrap
**```<header>```**
```
<header class="p-3">
  <h1 class="mt-2 mb-2 me-1 ms-1 text-body-tertiary fw-bold">Layout Sederhana</h1>
</header>
```
**```<body>**
```
<body class="text-body-secondary lh-1">
```
**```<div class="container">```**
```
<div class="container w-75 shadow-lg p-3 mb-0 bg-body-tertiary rounded" id="container">
```
**```<nav>```dan```<a>``` pada Navigasi**
```
<nav class="bg-primary d-block"> 
  <a href="#" class="active pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">Home</a>
  <a href="#article" class="active pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">Artikel</a>
  <a href="#about" class="active pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">About</a>
  <a href="#contact" class="active pt-3 pb-3 ps-3 pe-3 text-white fs-6 fw-bold text-decoration-none d-inline-block">Kontak</a>
</nav>
```
**```<section id="hero">```**
```
<section id="hero" class="bg-dark-subtle pb-5 pt-5 pe-3 ps-3 mb-2">
```
**```<div id=""wrapper">```**
```
<div id="wrapper" class="m-0 position-relative">
```
**```<section id="main">```**
```
<section id="main" class="float-start w-75 p-2 ">
```
**```<div class="box">```**
```
<div class="box" class="box pt-0 pb-0 pe-2 d-block float-none w-25">
```
**```<img>```**
```
<img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="rounded-circle ms-4">
```
**```<h3>```pada```<div class="box">```**
```
<h3 class="mt-2 mb-2 me-0 ms-0 text-center fs-4 fw-bold">Heading</h3>
```
**```<p>``` pada ```<div class="box">```**
```
<p class="lh-base fs-6 mb-2 text-center">Donec sed odio dui. Etiam porta sem malesuada magna molliseuismod.</p>
```
**```<a>``` pada ```<div class="box">```**
```
<a href="#" class="ms-5 fw-medium fs-6 btn bg-dark-subtle p-2 rounded">View detail</a>
```
**```<hr>```**
```
<hr class="divider border-0 border-top border-light-subtle mb-3 mt-3 me-0 ms-0">
```
**```<article>```**
```
<article class="entry mb-2 mt-2 me-0 ms-0" id="article">
```
**```<img>``` pada ```<article>```**
```
<img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="float-start rounded ms-2">
```
**```<p>``` pada ```<article>```**
```
<p class="lh-base">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum loremelit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nuncpretium ac.</p>
```
**```<aside id="sidebar">```**
```
<aside id="sidebar" class="float-start w-25 p-3">
```
**```<div>``` pada ```<aside>```**
```
<div class="widget-box border border-secondary mb-3">
```
**```<h3>``` pada ```<aside>```**
```
<h3 class="title pt-2 pb-2 ps-2 pe-2 bg-primary text-white fs-4">Widget Header</h3>
```
**```<ul>``` pada ```<aside>```**
```
<ul class="list-unstyled">
```
**```<li>``` pada ```<aside>```**
```
<li class="border-bottom border-secondary">
```
**```<a>``` pada```<aside>```**
```
<a href="#" class="pt-2 pb-2 pe-3 ps-3 text-success-emphasis d-block text-decoration-none">Widget Link</a>
```
**```<div class="widget"```>**
```
div class="widget-box border border-secondary mb-3">
```
**```<h3>``` pada ```<div id="widget"```**
```
<h3 class="title pt-2 pb-2 ps-2 pe-2 bg-primary text-white fs-4">Widget Text</h3>
```
**```<p>```pada ```<div id="widget">```**
```
<p class="p-2 lh-base">Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tinciduntarcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integerpharetra est nunc, nec pretium nunc pretium ac.</p>
```
**```<footer>```**
```
<footer class="w-75 text-white bg-dark mx-auto p-2 text-center">
```

# Import Bundle Bottstrap Js
Masukkan kode 
```
<script>
  feather.replace();
</script>
```
```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
```
