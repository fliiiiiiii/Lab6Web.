# Praktikum Modul Pemrograman Web 1
Nama : AFLAH ATHALLAH TAMAM KAPUKONG

NIM : 312410280

KELAS : TI.24.A.4

# TUGAS & PERTANYAAN

1. Refactor Layout Praktikum 4
Ambil layout web sederhana dari Praktikum 4. Buat ulang layout tersebut menggunakan
Bootstrap Grid System.
○ Gunakan <nav> Bootstrap untuk bagian navigasi
○ Gunakan class .row dan .col-md-8 untuk main content dan .col-md-4 untuk sidebar
○ Gunakan komponen .card Bootstrap untuk menggantikan .widget-box
○ Gunakan komponen .card untuk menggantikan .box (bagian "Heading" yang berisi 3
kolom)
○ Anda tidak diperbolehkan menggunakan CSS float atau clear manual.

```
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Layout Praktikum 4 (Bootstrap)</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- NAVBAR -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container">
      <a class="navbar-brand" href="#">MyWebsite</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navbarNav" class="collapse navbar-collapse">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#">About</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- MAIN CONTENT + SIDEBAR -->
  <div class="container my-4">
    <div class="row">
      <!-- MAIN CONTENT -->
      <div class="col-md-8">
        <div class="card mb-4">
          <div class="card-body">
            <h3 class="card-title">Judul Konten Utama</h3>
            <p class="card-text">Ini adalah contoh isi konten utama. Kamu bisa menambahkan teks, gambar, atau artikel di sini.</p>
          </div>
        </div>
      </div>

      <!-- SIDEBAR -->
      <div class="col-md-4">
        <div class="card mb-4">
          <div class="card-header">Sidebar</div>
          <div class="card-body">
            <p>Ini area sidebar. Bisa untuk menu tambahan, informasi, atau widget.</p>
          </div>
        </div>
      </div>
    </div>

    <!-- TIGA KOTAK (HEADING / BOX) -->
    <div class="row mt-4">
      <div class="col-md-4">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Box 1</h5>
            <p class="card-text">Deskripsi singkat.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Box 2</h5>
            <p class="card-text">Deskripsi singkat.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Box 3</h5>
            <p class="card-text">Deskripsi singkat.</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

#OUTPUT

![gambar](https://github.com/fliiiiiiii/Lab6Web./blob/c9b8331ac87fff116784789a7666296da1bc520e/image/Screenshot%202025-10-30%20134218.png)

2. Refactor Form Praktikum 5
Ambil salah satu form dari Praktikum 5 (misalnya Form Input 23atau Form Button 24).
Buat ulang form tersebut agar terlihat rapi menggunakan class-class form Bootstrap (.form-
control, .form-label, .btn).

```
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Form Praktikum 5 (Bootstrap)</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light">

  <div class="container py-5">
    <div class="row justify-content-center">
      <div class="col-md-6">
        <div class="card shadow">
          <div class="card-header bg-primary text-white text-center">
            <h4>Form Input Data</h4>
          </div>
          <div class="card-body">
            <form>
              <div class="mb-3">
                <label for="nama" class="form-label">Nama Lengkap</label>
                <input type="text" id="nama" class="form-control" placeholder="Masukkan nama Anda">
              </div>

              <div class="mb-3">
                <label for="email" class="form-label">Email</label>
                <input type="email" id="email" class="form-control" placeholder="nama@email.com">
              </div>

              <div class="mb-3">
                <label for="pesan" class="form-label">Pesan</label>
                <textarea id="pesan" class="form-control" rows="3" placeholder="Tulis pesan Anda"></textarea>
              </div>

              <button type="submit" class="btn btn-success w-100">Kirim</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>

</body>
</html>
```

#OUTPUT 

![gambar](https://github.com/fliiiiiiii/Lab6Web./blob/c9b8331ac87fff116784789a7666296da1bc520e/image/Screenshot%202025-10-30%20134257.png)

3. Tugas: Buat Halaman Portfolio Sederhana
Buat satu halaman HTML baru (portfolio.html) menggunakan Bootstrap yang berisi:
a. Sebuah Navbar di bagian atas.
b. Sebuah section "Tentang Saya" di dalam .container dengan 1 baris (.row) dan 2 kolom
(.col):
* Kolom kiri (.col-md-4) berisi foto Anda (gunakan <img> dengan class .img-fluid).
* Kolom kanan (.col-md-8) berisi nama dan deskripsi diri Anda.
c. Sebuah section "Portfolio Saya" di dalam .container dengan 1 baris (.row) dan 3 kolom
(.col-md-4):
* Setiap kolom berisi satu komponen .card yang merepresentasikan satu proyek (beri
gambar dummy dan deskripsi singkat).

```
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Portfolio Afii</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container">
      <a class="navbar-brand" href="#">Afii Portfolio</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navMenu" class="collapse navbar-collapse">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#tentang">Tentang</a></li>
          <li class="nav-item"><a class="nav-link" href="#portfolio">Portfolio</a></li>
          <li class="nav-item"><a class="nav-link" href="#kontak">Kontak</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Tentang Saya -->
  <section id="tentang" class="container my-5">
    <div class="row align-items-center">
      <div class="col-md-4 text-center">
        <img src="pepek.jpg" class="img-fluid rounded-circle" alt="Foto Afii">
      </div>
      <div class="col-md-8">
        <h2>Rafli Anugrah (Afii)</h2>
        <p>Halo! Aku Afii, seorang mahasiswa yang suka belajar hal baru di dunia web development. Aku punya minat besar di front-end design dan selalu berusaha bikin tampilan web yang rapi dan interaktif.</p>
      </div>
    </div>
  </section>

  <!-- Portfolio Saya -->
  <section id="portfolio" class="container my-5">
    <h3 class="text-center mb-4">Portfolio Saya</h3>
    <div class="row g-4">
      <div class="col-md-4">
        <div class="card h-100">
          <img src="Screenshot 2025-09-04 164917.png" class="card-img-top" alt="Proyek 1">
          <div class="card-body">
            <h5 class="card-title">Proyek 1</h5>
            <p class="card-text">Website sederhana dengan tampilan responsive menggunakan Bootstrap.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card h-100">
          <img src="WhatsApp Image 2025-10-30 at 13.55.52_bd5a3fa0.jpg" class="card-img-top" alt="Proyek 2">
          <div class="card-body">
            <h5 class="card-title">Proyek 2</h5>
            <p class="card-text">Aplikasi pengingat sholat berbasis web dengan fitur alarm otomatis.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card h-100">
          <img src="Screenshot 2025-09-19 135544.png" class="card-img-top" alt="Proyek 3">
          <div class="card-body">
            <h5 class="card-title">Proyek 3</h5>
            <p class="card-text">Sistem manajemen data mahasiswa dengan CRUD sederhana.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="bg-dark text-white text-center py-3">
    <p>&copy; 2025 Afii | Dibuat dengan ❤️ dan Bootstrap</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

#OUTPUT

![gambar](https://github.com/fliiiiiiii/Lab6Web./blob/c9b8331ac87fff116784789a7666296da1bc520e/image/Screenshot%202025-10-30%20135732.png)
