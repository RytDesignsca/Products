
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="description" content="Product Page - RYT DESIGNS" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Products - RYT DESIGNS</title>
  <style>
    * {margin:0; padding:0; box-sizing:border-box;}
    :root {
      --primary-bg: #ffffff;
      --secondary-bg: #f7f7f7;
      --header-footer-bg: #22232a;
      --text-color: #161623;
      --inverse-text-color: #ffffff;
      --accent: #009e97;
      --accent-gradient: linear-gradient(45deg, #009e97 40%, #1bbfa8 100%);
      --shadow: 0 4px 24px rgba(30,40,70,0.09);
      --radius: 15px;
    }
    body {
      background-color: var(--primary-bg);
      color: var(--text-color);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      min-height: 100vh;
    }
    a {
      color: var(--accent);
      text-decoration: none;
      transition: color 0.18s;
    }
    a:hover { color: #14635c; }
    header {
      background: var(--header-footer-bg);
      padding: 1.7rem 1rem 1.2rem 1rem;
      text-align: center;
      color: var(--inverse-text-color);
      border-bottom-left-radius: var(--radius);
      border-bottom-right-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    header h1 {font-size:2.2rem; letter-spacing:1px;}
    .products-section {
      max-width: 1300px;
      margin: 3rem auto 1.5rem auto;
      padding: 2rem 1rem 1.7rem 1rem;
      background: var(--secondary-bg);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    .section-title {
      text-align:center;
      font-size:2.1rem;
      margin-bottom:2.5rem;
      letter-spacing:0.5px;
      font-weight: 700;
      color: var(--accent);
    }
    .products-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 2.2rem;
      justify-content: center;
    }
    .product-card {
      background: var(--primary-bg);
      border-radius: var(--radius);
      box-shadow: 0 2px 16px rgba(0,0,0,0.07), 0 0.5px 1px rgba(0,0,0,0.01);
      width: 270px;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 1.1rem 1rem 1.6rem 1rem;
      position: relative;
      transition: transform 0.19s, box-shadow 0.20s;
    }
    .product-card:hover {
      transform: translateY(-6px) scale(1.025);
      box-shadow: 0 9px 40px rgba(0,85,79,0.08), 0 2px 10px rgba(0,0,0,0.05);
      z-index: 1;
    }
    .product-card img {
      width: 218px; height:145px; object-fit: cover;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.10);
      margin-bottom: 1rem;
      background: #f1f1f1;
      border: 2.5px solid #d2f4f2;
      transition: border .2s;
    }
    .product-card h3 {
      margin-bottom: 0.45rem;
      font-size: 1.15rem;
      color: #222;
      text-align: center;
      font-weight: 600;
      letter-spacing: 0.2px;
    }
    .product-card p {
      font-size: 1.02rem;
      margin-bottom: 1rem;
      min-height: 28px;
      text-align: center;
      color: #555;
    }
    .product-price {
      font-size: 1.21rem;
      font-weight: bold;
      letter-spacing: 0.5px;
      color: var(--accent);
      margin-bottom: 1rem;
    }
    .product-actions {
      display: flex;
      gap: 0.5rem;
      flex-wrap: wrap;
      width: 100%;
      justify-content: center;
    }
    .product-actions button {
      padding: 0.67rem 1.3rem;
      border: none;
      color: var(--inverse-text-color);
      background: var(--accent-gradient);
      font-size: 1rem;
      font-weight: 600;
      cursor: pointer;
      border-radius: 6px;
      letter-spacing: 0.3px;
      transition: filter 0.18s, transform 0.12s;
      box-shadow: 0 2.5px 6px rgba(0,158,151,0.10);
    }
    .product-actions button.buy-btn {
      box-shadow: 0 6.5px 16px rgba(0,158,151,0.16);
    }
    .product-actions button:hover {
      filter: brightness(0.91);
      transform: translateY(-1.6px) scale(1.035);
    }

    /* Cart Floating Panel */
    .cart-panel {
      position: fixed;
      top: 52px;
      right: 3vw;
      width: 350px;
      max-width: 96vw;
      background: #fff;
      color: #222;
      box-shadow: 0 8px 28px rgba(0,60,90,0.13);
      border-radius: 14px;
      padding: 1.09rem 1.1rem 1.4rem 1.1rem;
      z-index: 30;
      display: none;
      flex-direction: column;
      min-height: 80px;
      min-width: 280px;
      border-top: 6px solid var(--accent);
      border-right: 2.5px solid #96e7e6;
      border-bottom: 2px solid #effffd;
      animation: fadeInCart 0.25s linear;
    }
    @keyframes fadeInCart {
      from { opacity: 0; transform: translateY(-40px) scale(.92);}
      to { opacity: 1; transform: translateY(0) scale(1);}
    }
    .cart-panel-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 1.22rem;
      font-weight: 600;
      margin-bottom: 0.8rem;
      color: var(--accent);
      letter-spacing: 0.2px;
    }
    .cart-panel-close {
      background: none;
      border: none;
      color: #888;
      font-size: 1.4rem;
      cursor: pointer;
      transition: color 0.18s;
    }
    .cart-panel-close:hover { color: #ff5252; }
    .cart-list {
      margin: 0.1rem 0 0.8rem 0;
      padding: 0;
      list-style: none;
      max-height: 290px;
      overflow-y: auto;
      scrollbar-width: thin;
    }
    .cart-list li {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: .38rem 0;
      border-bottom: 1.7px dashed #e8eeeb;
      font-size: 1rem;
      gap: 0.6rem;
    }
    .cart-list .cart-productTitle {
      flex:2;
      word-break:break-word;
      font-weight:500;
      color: #333;
    }
    .cart-list .cart-item-qty {
      display: flex; gap: 0.22em; align-items: center;
    }
    .cart-list .qty-btn {
      width: 1.6em; height:1.6em;
      background: #ecf9f5;
      color: var(--accent);
      border:none; border-radius:4px;
      font-size:1.13rem; font-weight:700;
      cursor:pointer;
      display: flex; align-items: center; justify-content:center;
      transition: background 0.17s;
    }
    .cart-list .qty-btn:hover { background: #b1f6ee; }
    .cart-list .delete-btn {
      background: none;
      color: #ee6352;
      border: none;
      font-size: 1.18em;
      cursor: pointer;
      margin-left: 0.35em;
      padding: 0;
      transition: color 0.2s;
    }
    .cart-list .delete-btn:hover { color: #b10017;}
    .cart-total-row {
      display: flex;
      justify-content: space-between;
      font-size: 1.1rem;
      font-weight: 600;
      margin-top: 1em;
      padding-top: .63em;
      border-top: 2.2px solid #def8f5;
    }
    .empty-cart {
      color: #999;
      font-size: 1.1em;
      text-align: center;
      margin: 1.1em 0;
    }
    .cart-btn-floating {
      appearance: none;
      outline: none;
      border: none;
      border-radius: 50%;
      background: var(--accent-gradient);
      color: #fff;
      position: fixed;
      top: 2.35rem; right: 2.5vw;
      width: 62px; height: 62px;
      font-size: 2.1rem;
      display: flex; align-items: center; justify-content: center;
      z-index: 1011;
      box-shadow: 0 0 22px 2px rgba(25,185,163,0.13);
      cursor: pointer;
      transition: background .18s, box-shadow .18s, transform .16s;
      box-shadow: 0 8px 18px rgba(0,158,151,0.13);
      border-bottom: 7px solid #aeefee;
    }
    .cart-btn-floating.invert {
      background: #fff;
      color: var(--accent);
      border: 1.5px solid var(--accent);
      border-bottom: 7px solid #aeefee;
    }
    .cart-btn-floating.badge:after {
      content: attr(data-cart-count);
      position: absolute;
      top: 7px; right: 8px;
      font-size: 1.07em;
      background: #1fcba7;
      color: #fff;
      border-radius: 50%;
      padding: 0 7px;
      font-weight: 700;
      border: 2px solid #fff;
      box-shadow: 0 1.2px 5px rgba(0,80,100,0.16);
      letter-spacing:0.1px;
      pointer-events:none;
    }
    @media (max-width:600px){
      .products-section { padding: 1.3rem 1vw 1.3rem 1vw; margin: 1.2rem auto;}
      .products-grid {gap: 1.12rem;}
      .cart-panel { width:96vw; max-width:100vw; right:2vw; padding: 0.7rem 0.7rem 1.2rem 0.7rem;}
      .cart-btn-floating { right: 1vw; }
      header {font-size:1.1em;}
    }
    footer {
      margin-top:2rem;
      background-color: var(--header-footer-bg);
      text-align: center;
      padding: 1.1rem 1rem;
      color: var(--inverse-text-color);
      border-top-left-radius: var(--radius);
      border-top-right-radius: var(--radius);
      font-size:1.06em;
    }
    footer a { color: var(--accent); text-decoration: none; font-weight: bold;}
    footer a:hover { color: var(--inverse-text-color);}
  </style>
</head>
<body>
  <header>
    <h1>Products - RYT DESIGNS</h1>
  </header>
  <button class="cart-btn-floating badge" id="cartBtn" title="Show Cart" data-cart-count="0" onclick="openCart()">
    🛒
  </button>
  <div class="cart-panel" id="cartPanel">
    <div class="cart-panel-header">
      <span>Your Cart</span>
      <button class="cart-panel-close" onclick="closeCart()" title="Close">&times;</button>
    </div>
    <ul class="cart-list" id="cartList"></ul>
    <div class="cart-total-row">
      <span>Total:</span>
      <span id="cartTotal">$0</span>
    </div>
  </div>
  <section class="products-section">
    <div class="section-title">Our Products &amp; Services</div>
    <div class="products-grid">

      <div class="product-card">
        <img src="rytdesignsca-products-page/website/Album cover.png" alt="Album Cover Design" />
        <h3>Album Cover</h3>
        <p>Create custom album or song cover designs tailored to your music.</p>
        <div class="product-price">$20</div>
        <div class="product-actions">
          <button class="buy-btn" onclick="buyNow('Album Cover', 20)">Buy Now</button>
          <button onclick="addToCart('Album Cover', 20)">Add to Cart</button>
        </div>
      </div>

      <div class="product-card">
        <img src="rytdesignsca-products-page/website/Banner 4 website.png" alt="Banner Design" />
        <h3>Banner Design</h3>
        <p>Custom banners perfect for campaigns or announcements.</p>
        <div class="product-price">$35</div>
        <div class="product-actions">
          <button class="buy-btn" onclick="buyNow('Banner Design', 35)">Buy Now</button>
          <button onclick="addToCart('Banner Design', 35)">Add to Cart</button>
        </div>
      </div>

      <div class="product-card">
        <img src="rytdesignsca-products-page/website/Logo 4 website.png" alt="Logo Design" />
        <h3>Logo Design</h3>
        <p>Professional branding with unique logos for businesses.</p>
        <div class="product-price">$30</div>
        <div class="product-actions">
          <button class="buy-btn" onclick="buyNow('Logo Design', 30)">Buy Now</button>
          <button onclick="addToCart('Logo Design', 30)">Add to Cart</button>
        </div>
      </div>

      <div class="product-card">
        <img src="rytdesignsca-products-page/website/Menu 4 website.png" alt="Menu Design" />
        <h3>Menu Design</h3>
        <p>Custom menus for restaurants or events.</p>
        <div class="product-price">$20</div>
        <div class="product-actions">
          <button class="buy-btn" onclick="buyNow('Menu Design', 20)">Buy Now</button>
          <button onclick="addToCart('Menu Design', 20)">Add to Cart</button>
        </div>
      </div>

      <!-- Add other product cards following the same pattern -->
    </div>
  </section>

  <footer>
    <p>&copy; 2025 RYT DESIGNS. All Rights Reserved.</p>
    <p><a href="index.html">Back to Home</a></p>
  </footer>

  <script>
    let cart = [];

    function updateCartBadge() {
      const badge = document.getElementById('cartBtn');
      const count = cart.reduce((sum, item) => sum + item.quantity, 0);
      badge.setAttribute('data-cart-count', count);
    }

    function renderCart() {
      const cartList = document.getElementById('cartList');
      const cartTotal = document.getElementById('cartTotal');
      cartList.innerHTML = "";
      let total = 0;

      if (cart.length === 0) {
        cartList.innerHTML = `<div class="empty-cart">Your cart is empty.</div>`;
      } else {
        cart.forEach((item, idx) => {
          total += item.price * item.quantity;
          cartList.innerHTML += `
            <li>
              <span class="cart-productTitle">${item.name}</span>
              <span class="cart-item-qty">
                <button class="qty-btn" onclick="changeQty(${idx},-1)">-</button>
                <span class="qty-number">${item.quantity}</span>
                <button class="qty-btn" onclick="changeQty(${idx},1)">+</button>
              </span>
              <span class="cart-item-price">$${item.price * item.quantity}</span>
              <button class="delete-btn" onclick="removeFromCart(${idx})" title="Remove">&times;</button>
            </li>
          `;
        });
      }
      cartTotal.textContent = `$${total}`;
      updateCartBadge();
    }

    function addToCart(name, price) {
      const existing = cart.find(item => item.name === name);
      if (existing) {
        existing.quantity += 1;
      } else {
        cart.push({ name, price, quantity: 1 });
      }
      renderCart();
      updateCartBadge();
      openCart();
    }

    function removeFromCart(idx) {
      cart.splice(idx, 1);
      renderCart();
      updateCartBadge();
    }

    function changeQty(idx, amt) {
      const item = cart[idx];
      if (!item) return;
      item.quantity += amt;
      if (item.quantity < 1) {
        removeFromCart(idx);
      } else {
        renderCart();
        updateCartBadge();
      }
    }

    function openCart() {
      document.getElementById('cartPanel').style.display = 'flex';
      renderCart();
    }

    function closeCart() {
      document.getElementById('cartPanel').style.display = 'none';
    }

    // Clicking outside closes cart
    document.addEventListener('click', function(e) {
      const cartPanel = document.getElementById('cartPanel');
      const cartBtn = document.getElementById('cartBtn');
      if (cartPanel.style.display === 'flex' && !cartPanel.contains(e.target) && !cartBtn.contains(e.target)) {
        closeCart();
      }
    });

    // ESC closes cart
    document.addEventListener('keydown', function(e) {
      if (e.key === "Escape") closeCart();
    });

    function buyNow(name, price) {
      addToCart(name, price);
      alert(`Proceeding to buy ${name} for $${price}.`);
    }

    // On load, initialize badge
    updateCartBadge();
  </script>
</body>
</html>
