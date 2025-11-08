<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>BonekaMySya — Boneka Lucu & Berkualitas</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#fbfbfd; --card:#ffffff; --muted:#6b7280; --accent:#7c3aed; --accent-2:#a78bfa;
      --radius:14px; --shadow: 0 8px 30px rgba(17,24,39,0.08);
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:var(--bg);color:#0f172a;line-height:1.5}
    .container{max-width:1100px;margin:40px auto;padding:28px}

    /* Header */
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:32px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:52px;height:52px;border-radius:12px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:flex;align-items:center;justify-content:center;color:white;font-weight:700}
    nav a{margin-left:20px;color:var(--muted);text-decoration:none}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:32px;align-items:center}
    .kicker{color:var(--muted);font-size:14px;margin-bottom:10px}
    h1{font-size:40px;margin:0 0 16px 0;line-height:1.05}
    p.lead{color:var(--muted);max-width:560px}
    .cta{margin-top:22px;display:flex;gap:12px}
    .btn{padding:12px 18px;border-radius:10px;border:0;cursor:pointer;font-weight:600}
    .btn-primary{background:var(--accent);color:white;box-shadow:0 8px 22px rgba(124,58,237,0.16)}
    .btn-ghost{background:transparent;border:1px solid #e6e6f0;color:var(--muted)}

    .hero-card{background:var(--card);border-radius:var(--radius);box-shadow:var(--shadow);padding:18px}
    .hero-img{width:100%;height:540px;object-fit:cover;border-radius:12px}

    /* Feature pills */
    .features{display:flex;gap:14px;margin-top:22px}
    .pill{background:var(--card);padding:14px;border-radius:12px;box-shadow:0 6px 18px rgba(15,23,42,0.04);min-width:160px}
    .pill h4{margin:0 0 6px 0}
    .pill p{margin:0;color:var(--muted);font-size:14px}

    /* Produk grid */
    .produk{margin-top:44px}
    .produk-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{background:var(--card);border-radius:12px;padding:14px;box-shadow:var(--shadow);}
    .card img{width:100%;border-radius:8px;height:220px;object-fit:cover}
    .card h3{margin:10px 0 6px 0;font-size:18px}
    .card p{margin:0;color:var(--muted);font-size:14px}

    /* Gallery */
    .gallery{margin-top:42px;background:linear-gradient(180deg,#fff 0%, #fbfbfd 100%);padding:18px;border-radius:12px}
    .gallery-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:12px}
    .gallery img{width:100%;height:120px;object-fit:cover;border-radius:8px}

    footer{margin-top:44px;padding-top:18px;border-top:1px solid #f1f3f5;color:var(--muted);font-size:14px}

    /* Responsive */
    @media (max-width:980px){.hero{grid-template-columns:1fr 360px}.hero-img{height:380px}}
    @media (max-width:780px){.container{padding:18px;margin:20px auto}.hero{grid-template-columns:1fr;}.hero-img{height:300px}.produk-grid{grid-template-columns:1fr 1fr}.gallery-grid{grid-template-columns:repeat(2,1fr)}nav{display:none}}
    @media (max-width:420px){.produk-grid{grid-template-columns:1fr}.gallery-grid{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">FA</div>
        <div>
          <div style="font-weight:700">BonekaMySya</div>
          <div style="font-size:13px;color:var(--muted)">Cute • Soft • Handmade</div>
        </div>
      </div>
      <nav>
        <a href="#produk">Produk</a>
        <a href="#keunggulan">Keunggulan</a>
        <a href="#galeri">Galeri</a>
        <a href="#kontak">Kontak</a>
      </nav>
    </header>

    <!-- HERO -->
    <section class="hero">
      <div>
        <div class="kicker">Koleksi Terbaru • Gratis Ongkir</div>
        <h1>Boneka lucu, lembut, dan aman untuk semua usia</h1>
        <p class="lead">BonekaLova menghadirkan boneka berkualitas tinggi: berbahan lembut, jahitan rapi, dan desain menggemaskan. Cocok sebagai hadiah, koleksi, atau teman tidur untuk anak-anak.</p>
        <div class="cta">
          <button class="btn btn-primary">Belanja Sekarang</button>
          <button class="btn btn-ghost">Lihat Koleksi</button>
        </div>

        <div class="features">
          <div class="pill">
            <h4>Material Premium</h4>
            <p>Anti alergi, sangat lembut, mudah dicuci.</p>
          </div>
          <div class="pill">
            <h4>Handmade</h4>
            <p>Dijahit rapi oleh pengrajin berpengalaman.</p>
          </div>
          <div class="pill">
            <h4>Garansi 14 Hari</h4>
            <p>Tukar atau retur jika ada kerusakan.</p>
          </div>
        </div>
      </div>

      <aside class="hero-card">
        <!-- GANTI URL GAMBAR DENGAN FOTO PRODUKMU -->
        <img src="https://i.pinimg.com/736x/73/d0/b7/73d0b7a525eef730add1e5f7ffc16a10.jpg" alt="Boneka MySya - contoh" class="hero-img">
      </aside>
    </section>

    <!-- PRODUK PILIHAN -->
    <section id="produk" class="produk">
      <h2>Produk Pilihan</h2>
      <div class="produk-grid">
        <div class="card">
          <img src="https://i.pinimg.com/736x/ff/9d/f0/ff9df02e3be65a0519ae0c37fe252f0c.jpg" alt="Boneka Teddy">
          <h3>Teddy Plush - Mini</h3>
          <p>20 cm • Cocok untuk bayi • Harga Rp120.000</p>
        </div>
        <div class="card">
          <img src="https://i.pinimg.com/736x/86/5b/89/865b8991b1b8fa33c7ee8c21fa49e1bf.jpg" alt="Boneka Kelinci">
          <h3>Kelinci Bliss</h3>
          <p>30 cm • Bulu super lembut • Harga Rp165.000</p>
        </div>
        <div class="card">
          <img src="https://i.pinimg.com/736x/25/2d/13/252d134f009420cdaf03399855d25db7.jpg" alt="Boneka Custom">
          <h3>Boneka Custom</h3>
          <p>Custom nama & outfit • Pesan 7 hari kerja • Mulai Rp220.000</p>
        </div>
      </div>
    </section>

    <!-- GALERI -->
    <section id="galeri" class="gallery">
      <h2>Galeri</h2>
      <div class="gallery-grid">
        <img src="https://i.pinimg.com/1200x/04/cd/20/04cd209b8fc1b1a2ed7c643e7d98813f.jpg" alt="galeri1">
        <img src="https://i.pinimg.com/736x/40/a2/c0/40a2c0c574bcbe74a8fa41562d32ef03.jpg" alt="galeri2">
        <img src="https://i.pinimg.com/736x/4a/30/be/4a30be7dbefb7d0616b0bf8affcc8c06.jpg" alt="galeri3">
        <img src="https://i.pinimg.com/736x/b4/8b/5a/b48b5a64c3621f89d3e709997620a49f.jpg" alt="galeri4">
      </div>
    </section>

    <!-- KONTAK -->
    <section id="kontak" style="margin-top:28px;display:flex;gap:20px;align-items:flex-start;flex-wrap:wrap">
      <div style="flex:1;min-width:260px">
        <h3>Hubungi Kami</h3>
        <p style="color:var(--muted)">Pesan custom, pertanyaan produk, atau kerja sama — kami siap membantu.</p>
        <p style="margin-top:12px"><strong>WhatsApp:</strong> +62 858-1097-543<br><strong>Email:</strong> Fasya@BonekaMySya.id</p>
      </div>
      <form style="flex:1;min-width:260px;background:var(--card);padding:14px;border-radius:12px;box-shadow:var(--shadow)">
        <label style="display:block;margin-bottom:8px;color:var(--muted)">Nama</label>
        <input placeholder="Nama" style="width:100%;padding:10px;border-radius:8px;border:1px solid #eef2ff;margin-bottom:10px">
        <label style="display:block;margin-bottom:8px;color:var(--muted)">Pesan</label>
        <textarea placeholder="Tulis pesan" style="width:100%;padding:10px;border-radius:8px;border:1px solid #eef2ff;min-height:90px"></textarea>
        <div style="margin-top:10px;text-align:right">
          <button class="btn btn-primary" type="button">Kirim Pesan</button>
        </div>
      </form>
    </section>

    <footer>
      <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap">
        <div>© 2025 BonekaMySya • All rights reserved</div>
        <div style="color:var(--muted)">Desain sederhana — Siap untuk marketplace & Instagram</div>
      </div>
    </footer>
  </div>

  <script>
    // Contoh: tombol CTA scroll ke produk
    document.querySelectorAll('.btn-ghost, .btn-primary').forEach(btn => {
      btn.addEventListener('click', (e)=>{
        if(btn.textContent.includes('Lihat') || btn.textContent.includes('Pelajari')){
          location.hash = '#produk';
        } else if(btn.textContent.includes('Belanja')){
          // ganti dengan link toko atau keranjang
          window.location.href = '#kontak';
        }
      })
    })
  </script>
</body>
</html>
