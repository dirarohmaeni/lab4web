### Nama: Dira Rohmaeni
### NIM: 312410465
### Kelas: TI.24.A5

# Praktikum 4: CSS Layout
# Langkah-langkah Praktikum

1. Buat dokumen HTML dengan nama file lab4_box.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box Element</title>
  </head>
  <body>
    <header>
      <h1>Box Element</h1>
    </header>
  </body>
</html>
```
Lalu buka Browser untuk melihat hasilnya

2. Membuat Box Element
   Kemudian tambahkan kode untuk membuat box element dengan tag div
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box Element</title>
  </head>
  <body>
    <header>
      <h1>Box Element</h1>
    </header>

    <section>
      <div class="div1">Div 1</div>
      <div class="div2">Div 2</div>
      <div class="div3">Div 3</div>
    </section>
  </body>
</html>
```
Lalu buka Browser untuk melihat hasilnya

3. CSS Float Property
   Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element,
```css
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box Element</title>
  </head>
  <body>
    <header>
      <h1>Box Element</h1>
    </header>

    <section>
      <div class="div1">Div 1</div>
      <div class="div2">Div 2</div>
      <div class="div3">Div 3</div>
    </section>

    <style>
      div {
        float: left;
        padding: 10px;
      }
      .div1 {
        background: red;
      }
      .div2 {
        background: yellow;
      }
      .div3 {
        background: green;
      }
    </style>
  </body>
</html>
```
Lalu buka Browser untuk melihat hasilnya

4. Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.
Tambahkan element div lainnya seteleah div3
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box Element</title>
  </head>
  <body>
    <header>
      <h1>Box Element</h1>
    </header>

    <section>
      <div class="div1">Div 1</div>
      <div class="div2">Div 2</div>
      <div class="div3">Div 3</div>
      <div class="div4">Div 4</div>
    </section>

    <style>
      div {
        float: left;
        padding: 10px;
      }
      .div1 {
        background: red;
      }
      .div2 {
        background: yellow;
      }
      .div3 {
        background: green;
      }
    </style>
  </body>
</html>
```
Lalu buka Browser untuk melihat hasilnya

5. Kemudian atur property clear pada CSS,
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box Element</title>
  </head>
  <body>
    <header>
      <h1>Box Element</h1>
    </header>

    <section>
      <div class="div1">Div 1</div>
      <div class="div2">Div 2</div>
      <div class="div3">Div 3</div>
      <div class="div4">Div 4</div>
    </section>

    <style>
      div {
        float: left;
        padding: 10px;
      }
      .div1 {
        background: red;
      }
      .div2 {
        background: yellow;
      }
      .div3 {
        background: green;
      }
      .div4 {
        background-color: blue;
        clear: left;
        float: none;
      }
    </style>
  </body>
</html>
Lalu buka Browser untuk melihat hasilnya


1. Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama
home.html, dan file css dengan nama style.css.
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div id="container"></div>
  </body>
</html>
```
2. Kemudian tulis kode tersebut
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div id="container"></div>
    <header>
      <h1>Layout Sederhana</h1>
    </header>
    <nav>
      <a href="home.html" class="active">Home</a>
      <a href="artikel.html">Artikel</a>
      <a href="about.html">About</a>
      <a href="kontak.html">Kontak</a>
    </nav>
    <section id="hero"></section>
    <section id="wrapper">
      <section id="main"></section>
      <aside id="sidebar"></aside>
    </section>
    <footer>
      <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
  </body>
</html>
```
Lalu buka Browser untuk melihat hasilnya

3. Kemudian tambahkan kode CSS untuk membuat layoutnya.
```css
/* Import Google Fonts */
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap");

/* Reset CSS */
* {
  margin: 0;
  padding: 0;
}

/* Body */
body {
  line-height: 1;
  font-size: 100%;
  font-family: "Open Sans", sans-serif;
  color: #5a5a5a;
}

/* Container */
#container {
  width: 980px;
  margin: 0 auto;
  box-shadow: 0 0 1em #cccccc;
}

/* Header */
header {
  padding: 20px;
}

header h1 {
  margin: 20px 10px;
  color: #b5b5b5;
}
```
Lalu buka Browser untuk melihat hasilnya
4.  

 


