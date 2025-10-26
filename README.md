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
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/BOX/image1.png)

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
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/BOX/image2.png)

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
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/BOX/image3.png)

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

5. Kemudian atur property clear pada CSS,
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
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/BOX/image4.png)

6. Both
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/BOX/H-both.png)

7. Right
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/BOX/H-right.png)

# Membuat Layout Sederhana
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
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/HOME/HASIL1-home.png)

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
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%201.png)

4. Kemudian selanjutnya mengatur navigasi.
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%202.png)


5. Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS
### html
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

    <section id="hero">
      <h1>Hello World!</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
        lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in
        leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est
        nunc, nec pretium nunc pretium ac.
      </p>
      <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

    <footer>
      <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
  </body>
</html>
```
### CSS
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

/* Hero Panel */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 {
  margin-bottom: 20px;
  font-size: 35px;
}
#hero p {
  margin-bottom: 20px;
  font-size: 18px;
  line-height: 25px;
}
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%203.png)

6. Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

/* Hero Panel */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 {
  margin-bottom: 20px;
  font-size: 35px;
}
#hero p {
  margin-bottom: 20px;
  font-size: 18px;
  line-height: 25px;
}

/* main content */
#wrapper {
  margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: right;
  width: 260px;
  padding: 20px;
}
```
Kemudian selanjutnya menambahkan element lain dalam sidebar.
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

    <section id="hero">
      <h1>Hello World!</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
        lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in
        leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est
        nunc, nec pretium nunc pretium ac.
      </p>
      <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

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
        <p>
          Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
          arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis.
          Integer pharetra est nunc, nec pretium nunc pretium ac.
        </p>
      </div>
    </aside>
  </body>
</html>
```
Kemudian tambahkan CSS.
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

/* Hero Panel */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 {
  margin-bottom: 20px;
  font-size: 35px;
}
#hero p {
  margin-bottom: 20px;
  font-size: 18px;
  line-height: 25px;
}

/* main content */
#wrapper {
  margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: right;
  width: 260px;
  padding: 20px;
}

/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
.widget-box li a {
  padding: 10px 16px;
  color: #333;
  display: block;
  text-decoration: none;
}
.widget-box li:hover a {
  background-color: #eee;
}
.widget-box p {
  padding: 15px;
  line-height: 25px;
}
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%204.png)

7. Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

/* Hero Panel */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 {
  margin-bottom: 20px;
  font-size: 35px;
}
#hero p {
  margin-bottom: 20px;
  font-size: 18px;
  line-height: 25px;
}

/* main content */
#wrapper {
  margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: right;
  width: 260px;
  padding: 20px;
}

/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
.widget-box li a {
  padding: 10px 16px;
  color: #333;
  display: block;
  text-decoration: none;
}
.widget-box li:hover a {
  background-color: #eee;
}
.widget-box p {
  padding: 15px;
  line-height: 25px;
}

/* footer */
footer {
  clear: both;
  background-color: #1d1d1d;
  padding: 20px;
  color: #eee;
}
```
### html
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

    <section id="hero">
      <h1>Hello World!</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
        lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in
        leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est
        nunc, nec pretium nunc pretium ac.
      </p>
      <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

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
        <p>
          Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
          arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis.
          Integer pharetra est nunc, nec pretium nunc pretium ac.
        </p>
      </div>
    </aside>
    <footer>
      <p>&copy; 2025 - Universitas Pelita Bangsa</p>
    </footer>
  </body>
</html>
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%205.png)

8. Menambahkan Elemen lainnya pada Main Content
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

    <section id="hero">
      <h1>Hello World!</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
        lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in
        leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est
        nunc, nec pretium nunc pretium ac.
      </p>
      <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

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
        <p>
          Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
          arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis.
          Integer pharetra est nunc, nec pretium nunc pretium ac.
        </p>
      </div>
    </aside>

    <section id="main">
      <div class="row">
        <div class="box">
          <img
            src="https://dummyimage.com/120/db7d25/fff.png"
            alt=""
            class="image-circle"
          />
          <h3>Heading</h3>
          <p>
            Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.
          </p>
          <a href="#" class="btn btn-default">View detail</a>
        </div>
        <div class="box">
          <img
            src="https://dummyimage.com/120/3e73e6/fff.png"
            alt=""
            class="image-circle"
          />
          <h3>Heading</h3>
          <p>
            Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.
          </p>
          <a href="#" class="btn btn-default">View detail</a>
        </div>
        <div class="box">
          <img
            src="https://dummyimage.com/120/71e6d4/fff.png"
            alt=""
            class="image-circle"
          />
          <h3>Heading</h3>
          <p>
            Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.
          </p>
          <a href="#" class="btn btn-default">View detail</a>
        </div>
      </div>
    </section>

    <footer>
      <p>&copy; 2025 - Universitas Pelita Bangsa</p>
    </footer>
  </body>
</html>
```
Kemudian tambahkan CSS.
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

/* Hero Panel */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 {
  margin-bottom: 20px;
  font-size: 35px;
}
#hero p {
  margin-bottom: 20px;
  font-size: 18px;
  line-height: 25px;
}

/* main content */
#wrapper {
  margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: right;
  width: 260px;
  padding: 20px;
}

/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
.widget-box li a {
  padding: 10px 16px;
  color: #333;
  display: block;
  text-decoration: none;
}
.widget-box li:hover a {
  background-color: #eee;
}
.widget-box p {
  padding: 15px;
  line-height: 25px;
}

/* footer */
footer {
  clear: both;
  background-color: #1d1d1d;
  padding: 20px;
  color: #eee;
}

/* box */
.box {
  display: block;
  float: left;
  width: 33.333333%;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  padding: 0 10px;
  text-align: center;
}
.box h3 {
  margin: 15px 0;
}
.box p {
  line-height: 20px;
  font-size: 14px;
  margin-bottom: 15px;
}
.box img {
  border: 0;
  vertical-align: middle;
}
.image-circle {
  border-radius: 50%;
}
.row {
  margin: 0 -10px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
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
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%206.png)

9. Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
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
    <div id="container">
      <header>
        <h1>Layout Sederhana</h1>
      </header>

      <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
      </nav>

      <section id="hero">
        <h1>Hello World!</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
          lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin
          in leo fringilla, vestibulum mi porta, faucibus felis. Integer
          pharetra est nunc, nec pretium nunc pretium ac.
        </p>
        <a href="#" class="btn btn-large">Learn more &raquo;</a>
      </section>

      <section id="wrapper">
        <section id="main">
          <div class="row">
            <div class="box">
              <img
                src="https://dummyimage.com/120/db7d25/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#" class="btn btn-default">View detail</a>
            </div>

            <div class="box">
              <img
                src="https://dummyimage.com/120/3e73e6/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#" class="btn btn-default">View detail</a>
            </div>
            <div class="box">
              <img
                src="https://dummyimage.com/120/71e6d4/fff.png"
                alt=""
                class="image-circle"
              />
              <h3>Heading</h3>
              <p>
                Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.
              </p>
              <a href="#" class="btn btn-default">View detail</a>
            </div>
          </div>

          <hr class="divider" />

          <article class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </article>

          <hr class="divider" />
          <article class="entry">
            <h2>Second featurette heading.</h2>
            <img
              src="https://dummyimage.com/150/7b8a70/fff.png"
              alt=""
              class="right-img"
            />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis. Integer pharetra est nunc, nec pretium nunc
              pretium ac.
            </p>
          </article>
        </section>

        <aside id="sidebar">
          <div class="widget-box">
            <h3 class="title">Widget Header</h3>
            <ul>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
              <li><a href="#">Widget Link</a></li>
            </ul>
          </div>

          <div class="widget-box">
            <h3 class="title">Widget Text</h3>
            <p>
              Vestibulum lorem elit, iaculis in nisl volutpat, malesuada
              tincidunt arcu. Proin in leo fringilla, vestibulum mi porta,
              faucibus felis.
            </p>
          </div>
        </aside>
      </section>

      <footer>
        <p>&copy; 2025 - Universitas Pelita Bangsa</p>
      </footer>
    </div>
  </body>
</html>
```
Kemudian tambahkan CSS.
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

/* navigasi */
nav {
  display: block;
  background-color: #1f5faa;
}
nav a {
  padding: 15px 30px;
  display: inline-block;
  color: #ffffff;
  font-size: 14px;
  text-decoration: none;
  font-weight: bold;
}
nav a.active,
nav a:hover {
  background-color: #2b83ea;
}

/* Hero Panel */
#hero {
  background-color: #e4e4e5;
  padding: 50px 20px;
  margin-bottom: 20px;
}
#hero h1 {
  margin-bottom: 20px;
  font-size: 35px;
}
#hero p {
  margin-bottom: 20px;
  font-size: 18px;
  line-height: 25px;
}

/* main content */
#wrapper {
  margin: 0;
}
#main {
  float: left;
  width: 640px;
  padding: 20px;
}
/* sidebar area */
#sidebar {
  float: right;
  width: 260px;
  padding: 20px;
}

/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
/* widget */
.widget-box {
  border: 1px solid #eee;
  margin-bottom: 20px;
}
.widget-box .title {
  padding: 10px 16px;
  background-color: #428bca;
  color: #fff;
}
.widget-box ul {
  list-style-type: none;
}
.widget-box li {
  border-bottom: 1px solid #eee;
}
.widget-box li a {
  padding: 10px 16px;
  color: #333;
  display: block;
  text-decoration: none;
}
.widget-box li:hover a {
  background-color: #eee;
}
.widget-box p {
  padding: 15px;
  line-height: 25px;
}

/* footer */
footer {
  clear: both;
  background-color: #1d1d1d;
  padding: 20px;
  color: #eee;
}

/* box */
.box {
  display: block;
  float: left;
  width: 33.333333%;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  padding: 0 10px;
  text-align: center;
}
.box h3 {
  margin: 15px 0;
}
.box p {
  line-height: 20px;
  font-size: 14px;
  margin-bottom: 15px;
}
.box img {
  border: 0;
  vertical-align: middle;
}
.image-circle {
  border-radius: 50%;
}
.row {
  margin: 0 -10px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
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

.divider {
  border: 0;
  border-top: 1px solid #eeeeee;
  margin: 40px 0;
}
/* entry */
.entry {
  overflow: auto;
  margin: 15px 0;
}
.entry h2 {
  margin-bottom: 20px;
}
.entry p {
  line-height: 25px;
}
.entry img {
  float: left;
  border-radius: 5px;
  margin: 0 15px 10px 0;
  width: 150px;
  height: 150px;
}
.entry .right-img {
  float: right;
  margin: 0 0 10px 15px;
  width: 150px;
  height: 150px;
}
```
Lalu buka Browser untuk melihat hasilnya
![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/CSS/HASIL%207.png)

10.      

 


