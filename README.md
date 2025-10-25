### Nama: Dira Rohmaeni
### NIM: 312410465
### Kelas: TI.24.A5

# Praktikum 4: CSS Layout
Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
2. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll


Jawab

1. <img src ="/hasil about.png" width="500">

2. ```html
   <!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Kontak - Layout Sederhana</title>
    <link rel="stylesheet" href="style.css" />
    <style>
      form {
        display: flex;
        flex-direction: column;
        gap: 10px;
        width: 100%;
      }
      input,
      textarea {
        padding: 10px;
        border: 1px solid #ccc;
        border-radius: 5px;
        font-family: "Open Sans", sans-serif;
      }
      button {
        background-color: #1f5faa;
        color: white;
        border: none;
        padding: 10px 15px;
        border-radius: 5px;
        font-weight: bold;
        cursor: pointer;
      }
      button:hover {
        background-color: #2b83ea;
      }
    </style>
  </head>

  <body>
    <div id="container">
      <header>
        <h1>Layout Sederhana</h1>
      </header>

      <nav>
        <a href="home.html">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html" class="active">Kontak</a>
      </nav>

      <section id="hero">
        <h1>Hubungi Kami</h1>
        <p>Silakan isi form di bawah ini untuk mengirim pesan kepada kami.</p>
      </section>

      <section id="wrapper">
        <section id="main">
          <article class="entry">
            <h2>Form Kontak</h2>
            <form action="#" method="post">
              <label for="nama">Nama:</label>
              <input
                type="text"
                id="nama"
                name="nama"
                placeholder="Masukkan nama Anda"
                required
              />

              <label for="email">Email:</label>
              <input
                type="email"
                id="email"
                name="email"
                placeholder="Masukkan email Anda"
                required
              />

              <label for="pesan">Pesan:</label>
              <textarea
                id="pesan"
                name="pesan"
                rows="5"
                placeholder="Tulis pesan Anda..."
                required
              ></textarea>

              <button type="submit">Kirim Pesan</button>
            </form>
          </article>
        </section>

        <aside id="sidebar">
          <div class="widget-box">
            <h3 class="title">Info Kontak</h3>
            <ul>
              <li>Email: info@kampus.com</li>
              <li>Telepon: (021) 1234567</li>
              <li>Alamat: Cikarang, Jawa Barat</li>
            </ul>
          </div>
        </aside>
      </section>

      <footer>
        <p>&copy; 2025 - Universitas Pelita Bangsa</p>
      </footer>
    </div>
  </body>
</html>

Lalu buka Browser untuk melihat hasilnya

![foto](https://github.com/dirarohmaeni/lab4web/blob/63339edbea263ad581902edabc18be4cb22be5a4/lab4/contact/hasil%20kontak.png)


