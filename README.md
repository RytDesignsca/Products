
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="description" content="Product Page - RYT DESIGNS" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Products - RYT DESIGNS</title>
  <style>
    :root {
      --bg: #f7fafc;
      --card-bg: #fff;
      --radius: 12px;
      --shadow: 0 8px 32px rgba(24,40,60,0.11);
      --shadow-hover: 0 10px 38px rgba(22,99,74,0.13);
      --primary: #008080;
      --primary-dark: #007269;
      --border: #e4e8ef;
    }
    html, body { margin: 0; padding: 0; }
    body {
      background: var(--bg);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #18203c;
      min-height: 100vh;
      padding: 0;
    }
    .top-bar {
      display: flex;
      align-items: center;
      gap: 1rem;
      margin-top: 2rem;
      margin-bottom: 2.2rem;
      max-width: 1220px;
      margin-left: auto;
      margin-right: auto;
      padding: 0 1.6rem;
    }
    .back-home {
      background: var(--primary);
      color: #fff;
      text-decoration: none;
      padding: .6rem 1.1rem;
      border-radius: 25px;
      font-weight: 500;
      font-size: 1.06em;
      transition: background 0.17s;
      letter-spacing: 0.3px;
      box-shadow: 0 1px 10px rgba(0,128,128,0.09);
      border: none;
      display: inline-block;
    }
    .back-home:hover { background: var(--primary-dark);}
    .cart-tiny {
      margin-left: auto;
      background: #fff;
      border-radius: 25px;
      padding: .5rem 1.1rem;
      box-shadow: 0 2px 8px #00808018;
      font-weight: 500;
      display: flex; align-items: center; gap:0.6em;
      color: #242f36;
      border: 1.5px solid #e4ebe9;
    }
    .cart-tiny span {
      font-size: 1.2em;
      font-weight: 600;
      color: var(--primary);
    }
    .section-title {
      text-align:center;
      font-size:2rem;
      margin-bottom:2.4rem;
      letter-spacing:0.3px;
      font-weight: 600;
      color: var(--primary);
    }
    .products-grid {
      max-width: 1220px;
      margin: 0 auto 3rem auto;
      display: flex;
      flex-wrap: wrap;
      gap: 2.2rem;
      justify-content: center;
      padding: 0 1.3rem;
    }
    .product-card {
      background: var(--card-bg);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      width: 320px; /* wider card as in screenshot */
      margin-bottom: .5rem;
      display: flex;
      flex-direction: column;
      align-items: stretch;
      transition: box-shadow .22s, transform .22s;
      border: 1.7px solid var(--border);
    }
    .product-card:hover {
      box-shadow: var(--shadow-hover);
      transform: translateY(-4px) scale(1.016);
      border-color: #b8eee4;
    }
    .product-img-wrap {
      width: 100%;
      height: 285px;
      background: #def4f5;
      display: flex;
      align-items: center;
      justify-content: center;
      border-top-left-radius: 12px;
      border-top-right-radius: 12px;
      overflow: hidden;
    }
    .product-img-wrap img {
      width: 101%;
      height: 100%;
      object-fit: cover;
      border-top-left-radius: 12px;
      border-top-right-radius: 12px;
      background: #eef7f4;
      display: block;
    }
    .product-card-content {
      padding: 1.1rem 1rem 1.3rem 1rem;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      min-height: 110px;
      gap: 15px;
    }
    .product-title {
      font-size: 1.1rem;
      font-weight: 600;
      margin-bottom: 4px;
      letter-spacing: 0.1px;
    }
    .whatsapp-btn-row {
      width: 100%;
      margin-top: 2px;
      margin-bottom: 9px;
      display: flex;
      align-items: flex-end;
      justify-content: flex-start;
    }
    .wa-btn {
      display: flex;
      align-items: center;
      gap: 3px;
      background: #000;
      padding: 5.2px 18px 5.2px 7px;
      border-radius: 34px;
      cursor: pointer;
      border: none;
      text-decoration: none;
      margin-right: 0;
      box-shadow: 0 2px 8px #288C2255;
      transition: background .17s;
    }
    .wa-btn:hover { background: #067444; }
    .wa-logo {
      width: 42px;
      height: 42px;
      display: inline-block;
      background: #fff;
      background-size: cover;
      border-radius: 50%;
      margin-right: 8px;
      border: 3.2px solid #25d366;
      box-shadow: 0 2px 12px #02591f29;
    }
    .wa-btn span {
      color: #fff;
      font-weight: 600;
      font-size: 1.22em;
      letter-spacing: 0.2px;
    }
    .wa-btn small {
      color: #36e6a9;
      font-size: .9em;
      font-weight: 500;
      margin-right: 6px;
    }
    /* for mobile */
    @media (max-width: 600px) {
      .products-grid { padding-left: 4vw;padding-right: 4vw; gap: 1.2rem;}
      .product-card { width: 97vw;}
      .product-img-wrap {height: 34vw;min-height: 150px;}
      .top-bar { padding: 0 2vw;}
      .section-title { font-size: 1.1rem;}
    }
  </style>
</head>
<body>
  <!-- Top navigation bar with Home and Cart summary -->
  <div class="top-bar">
    <a href="index.html" class="back-home">← Back to Homepage</a>
    <div class="cart-tiny" id="cartTiny">
      <svg width="22" height="22" style="margin-right:.35em" fill="none" viewBox="0 0 24 24"><path fill="#008080" d="M7 20c.828 0 1.5.672 1.5 1.5S7.828 23 7 23s-1.5-.672-1.5-1.5S6.172 20 7 20Zm10 0c.828 0 1.5.672 1.5 1.5s-.672 1.5-1.5 1.5-1.5-.672-1.5-1.5.672-1.5 1.5-1.5ZM7.204 16l.701-1.745h8.83a2 2 0 0 0 1.866-1.302l3.025-8.013A1 1 0 0 0 20.701 4H5.214L4.27 1.813A1 1 0 0 0 3.369 1H1a1 1 0 0 0 0 2h1.145l3.6 8.59-1.353 2.446A2.005 2.005 0 0 0 6 17h12a1 1 0 0 0 0-2H7.819l-.615-1.154ZM6.16 5h12.47l-2.525 6.693a1 1 0 0 1-.904.644H8.563a1 1 0 0 1-.903-.644L6.16 5Z"></path></svg>
      <span id="cartCount">0</span> in cart
    </div>
  </div>

  <div class="section-title">Our Products &amp; Services</div>
  <div class="products-grid">

    <div class="product-card">
      <div class="product-img-wrap">
        <img src="rytdesignsca-products-page/website/Album cover.png" alt="Album Cover" loading="lazy" />
      </div>
      <div class="product-card-content">
        <div class="product-title">Album Cover</div>
        <div class="whatsapp-btn-row">
          <a class="wa-btn" href="https://wa.me/1234567890?text=I'm%20interested%20in%20the%20Album%20Cover%20product" target="_blank">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" class="wa-logo">
            <small>Order On</small>
            <span>Whatsapp</span>
          </a>
        </div>
      </div>
    </div>

    <div class="product-card">
      <div class="product-img-wrap">
        <img src="rytdesignsca-products-page/website/Banner 4 website.png" alt="Banner" loading="lazy" />
      </div>
      <div class="product-card-content">
        <div class="product-title">Banner Design</div>
        <div class="whatsapp-btn-row">
          <a class="wa-btn" href="https://wa.me/1234567890?text=I'm%20interested%20in%20the%20Banner%20Design%20product" target="_blank">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" class="wa-logo">
            <small>Order On</small>
            <span>Whatsapp</span>
          </a>
        </div>
      </div>
    </div>

    <div class="product-card">
      <div class="product-img-wrap">
        <img src="rytdesignsca-products-page/website/Logo 4 website.png" alt="Logo Design" loading="lazy" />
      </div>
      <div class="product-card-content">
        <div class="product-title">Logo Design</div>
        <div class="whatsapp-btn-row">
          <a class="wa-btn" href="https://wa.me/1234567890?text=I'm%20interested%20in%20the%20Logo%20Design%20product" target="_blank">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" class="wa-logo">
            <small>Order On</small>
            <span>Whatsapp</span>
          </a>
        </div>
      </div>
    </div>

    <div class="product-card">
      <div class="product-img-wrap">
        <img src="rytdesignsca-products-page/website/Menu 4 website.png" alt="Menu Design" loading="lazy" />
      </div>
      <div class="product-card-content">
        <div class="product-title">Menu Design</div>
        <div class="whatsapp-btn-row">
          <a class="wa-btn" href="https://wa.me/1234567890?text=I'm%20interested%20in%20the%20Menu%20Design%20product" target="_blank">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" class="wa-logo">
            <small>Order On</small>
            <span>Whatsapp</span>
          </a>
        </div>
      </div>
    </div>

    <!-- Example of more products (copy/paste and replace image/title as needed) -->
    <div class="product-card">
      <div class="product-img-wrap">
        <img src="rytdesignsca-products-page/website/Product label.png" alt="Product Label" loading="lazy" />
      </div>
      <div class="product-card-content">
        <div class="product-title">Product Label</div>
        <div class="whatsapp-btn-row">
          <a class="wa-btn" href="https://wa.me/1234567890?text=I'm%20interested%20in%20the%20Product%20Label%20product" target="_blank">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" class="wa-logo">
            <small>Order On</small>
            <span>Whatsapp</span>
          </a>
        </div>
      </div>
    </div>

  </div>
  <script>
    // Simple cart logic so your homepage and product page share the cart (using localStorage)
    function updateCartTiny() {
      const cartCount = JSON.parse(localStorage.getItem('rytCart') || '[]')
        .reduce((sum, item) => sum + item.quantity, 0);
      document.getElementById('cartCount').textContent = cartCount;
    }
    updateCartTiny();
  </script>
</body>
</html>
