<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>RYT DESIGNS – Creativity in every pixel</title>
  <meta name="viewport" content="width=1000, initial-scale=1">
  <style>
    :root {
      --dark-bg: #282828;
      --main-bg: #fff;
      --box: #f2f2f2;
      --primary: #009688;
      --primary-dark: #016e5f;
      --accent: #424242;
      --border: #ddd;
      --rounded: 14px;
      --shadow-lg: 0 2px 32px 0 rgba(42,48,86,0.12);
    }
    html,body { height:100%; margin:0; }
    body { background: var(--main-bg); color:#181818; font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
    .container-main {
      min-height: 100vh;
      display: flex;
      flex-direction: row;
      max-width: 1400px;
      margin: 0 auto;
      background: var(--main-bg);
    }
    .main-area {
      flex: 1 1 0%;
      padding: 54px 44px 22px 54px;
      border-right: 2.5px solid var(--border);
      min-width: 0;
      display: flex;
      flex-direction: column;
      /*overflow: auto;*/
    }
    .title-main {
      font-size: 2.75rem;
      font-weight: 700;
      color: var(--primary);
      margin-right:2rem;
    }
    .subtitle {
      margin-top: 0.5rem;
      margin-bottom: 2.1rem;
      font-size: 1.18rem;
      color: #555;
      font-weight: 400;
      max-width: 410px;
      border-bottom: 1px solid #e0e0e0;
      padding-bottom: 1.35rem;
    }
    .search-row {
      display: flex; gap: 0;
      margin-bottom: 1.4rem;
      align-items: stretch;
      width: 380px;
      box-sizing: border-box;
    }
    .search-row input {
      flex:1; font-size:1.13em; border-radius: 30px 0 0 30px;
      border: 1.4px solid var(--border);
      padding: 0.7em 1.1em;
      background: #fff;
      outline:none;
      border-right: 0;
      transition: border .13s;
    }
    .search-row input:focus { border-color: var(--primary-dark);}
    .search-row button {
      background: var(--accent);
      color: #fff;
      font-size: 1.11em;
      border: none;
      border-radius: 0 30px 30px 0;
      padding: 0 1.2em;
      cursor: pointer;
      font-weight: 600;
      transition: background 0.17s;
      letter-spacing:.05em;
    }
    .search-row button:hover {
      background: var(--primary-dark);
    }
    .popular-row {
      margin-bottom: 1.4rem; font-size: 15px;
      display: flex; gap:0.8rem; align-items: center;
      color: #5d5d61;
    }
    .popular-label { color: #616067; font-weight:500;}
    .popular-btn {
      background: var(--box);
      color: #222;
      border: none;
      border-radius: 9px;
      padding: 0.42em 1.18em;
      font-size: 1em;
      font-weight: 600;
      margin-right: 2px;
      cursor: pointer;
      transition: background .13s;
      box-shadow: 0 1.5px 8px #e1eee0;
    }
    .popular-btn:hover, .popular-btn.active { background: var(--primary); color: #fff;}
    .search-results-section {
      margin-top: 0.6em;
      min-height: 70px;
    }
    .result-card {
      margin-top: 10px;
      padding: 12px 14px;
      border-radius: 8px;
      box-shadow: 0 2px 24px #0218200a;
      background: #f7f7f9;
      font-size: 1.13em;
      display: flex;
      align-items: center;
      gap: 1.1em;
      justify-content:flex-start;
      max-width:370px;
      margin-bottom: 8px;
    }
    .result-title { font-weight: 600; font-size:1.07em;}
    .result-price { color: var(--primary); font-weight: 600; }
    .result-actions {
      display: flex; gap: 0.7em; margin-left: auto; align-items:center;
    }
    .buy-btn {
      background: var(--accent);
      color: #fff;
      border: none;
      border-radius: 8px;
      padding: 0.3em 1.25em;
      font-size:1em;
      font-weight: 600;
      cursor: pointer;
      transition: background .13s;
      margin-right: 0;
    }
    .buy-btn:hover { background: var(--primary-dark);}
    .preview-btn {
      background: #fff;
      border: 2px solid var(--primary);
      color: var(--primary);
      border-radius: 8px;
      padding: 0.3em 1.15em;
      font-size:1em;
      font-weight: 600;
      cursor: pointer;
      transition: background .13s, color .16s;
    }
    .preview-btn:hover { background: var(--primary); color: #fff;}
    /* Notification */
    .notif {
      position: fixed;
      left: 50%;
      top: 60px;
      z-index: 1000;
      transform: translateX(-50%) scale(0.9);
      background: var(--primary);
      color: #fff;
      padding: 16px 38px;
      border-radius: 18px;
      font-size: 1.13rem;
      box-shadow: 0 3px 21px #21412861;
      font-weight: 500;
      opacity: 0;
      pointer-events:none;
      transition: opacity 0.13s, transform 0.23s;
    }
    .notif.show {
      opacity: 1;
      pointer-events: all;
      transform: translateX(-50%) scale(1);
    }

    /* --- Cart Sidebar --- */
    .cart-sidebar {
      width: 310px;
      min-width: 310px;
      background: var(--dark-bg);
      color: #fff;
      padding: 0 24px;
      display: flex;
      flex-direction: column;
      align-items: stretch;
      min-height:100vh;
      box-sizing: border-box;
    }
    .cart-title {
      font-size: 1.41em;
      text-align:center;
      margin: 2rem 0 0.8rem 0;
      font-weight: 700;
      letter-spacing:.3px;
      padding-bottom: 6px;
      border-bottom: 2px solid #61606745;
    }
    .cart-items-list {
      margin: 17px 0 0 0;
      padding: 0;
      list-style: none;
      flex: 1 1 0;
    }
    .cart-item-box {
      background: #373739;
      border-radius: 10px;
      margin-bottom: 16px;
      box-shadow: 0 2px 14px #01010418;
      padding: 13px 14px 14px 18px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      font-size:1.05em;
    }
    .cart-item-desc {
      flex: 1 1 0;
      font-weight: 490;
      color: #f4fbf4;
      letter-spacing:.01px;
      font-size:1.06em;
    }
    .cart-item-remove {
      background: #222;
      color: #fff;
      border: none;
      font-size: 0.96em;
      font-weight: 500;
      border-radius: 7px;
      padding: 6px 12px;
      margin-left: 13px;
      cursor: pointer;
      transition: background .15s;
    }
    .cart-item-remove:hover {
      background: #e33b3b;
    }
    .cart-total-row {
      border-top: 1.7px solid #61606742;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 22px 0 11px 0;
      margin-top: 19px;
      font-size: 1.09em;
      font-weight: 500;
    }
    .cart-total-label { font-weight: 400;}
    .cart-checkout-btn {
      width: 100%;
      background: var(--primary);
      color: #fff;
      border: none;
      border-radius: 12px;
      font-size: 1.13em;
      font-weight: 600;
      padding: 14px 0 11px 0;
      cursor: pointer;
      margin-top: 16px;
      margin-bottom:17px;
      box-shadow:0 2px 12px #00808077;
      transition: background 0.11s;
    }
    .cart-checkout-btn:hover {
      background: var(--primary-dark);
    }
    @media (max-width: 1100px) {
      .container-main {
        flex-direction: column!important;
      }
      .main-area, .cart-sidebar {
        min-width: 0;
        width: 100%!important;
        border: none!important;
        box-sizing: border-box;
      }
      .cart-sidebar { min-height:0; }
      .main-area { border: none;}
    }
    @media (max-width: 650px) {
      .main-area { padding-left:3vw; padding-right:3vw;}
      .cart-sidebar { padding-left: 3vw; padding-right: 3vw;}
    }
  </style>
</head>
<body>
<div class="notif" id="cartNotif"></div>
<div class="container-main">
  <main class="main-area">
    <div class="title-main">Creativity in<br>every pixel</div>
    <div class="subtitle">Your Vision, My Creativity—Limitless Possibilities.</div>

    <form class="search-row" onsubmit="event.preventDefault(); onSearch();">
      <input id="searchInput" type="text" placeholder="Logo design" autocomplete="off" />
      <button type="submit">Get a design</button>
    </form>

    <div class="popular-row">
      <span class="popular-label">Popular:</span>
      <button class="popular-btn" onclick="quickSearch('Logo design')">Logo design</button>
      <button class="popular-btn" onclick="quickSearch('Website')">Website</button>
      <button class="popular-btn" onclick="quickSearch('Branding')">Branding</button>
    </div>

    <div id="searchResults" class="search-results-section"></div>
  </main>
  <aside class="cart-sidebar">
    <div class="cart-title">Your Cart</div>
    <ul id="cartList" class="cart-items-list"></ul>
    <div class="cart-total-row"><span class="cart-total-label">Total:</span> <span id="cartTotal">$0</span></div>
    <button class="cart-checkout-btn" onclick="onCheckout()">Checkout</button>
  </aside>
</div>
<script>
  // Products database
  const products = [
    {
      id: "logo-business",
      title: "Logos for businesses",
      price: 30,
      previewUrl: "products.html#logo-business"
    },
    {
      id: "poster-flyer",
      title: "Posters/Flyers",
      price: 15,
      previewUrl: "products.html#poster-flyer"
    },
    {
      id: "business-cards",
      title: "Business cards",
      price: 20,
      previewUrl: "products.html#business-cards"
    },
    {
      id: "invitation",
      title: "Invitations",
      price: 24,
      previewUrl: "products.html#invitation"
    },
    {
      id: "youtube-basic",
      title: "YouTube Thumbnails (Basic)",
      price: 20,
      previewUrl: "products.html#youtube-basic"
    },
    {
      id: "youtube-addon",
      title: "YouTube Thumbnail (Add-ons)",
      price: 35,
      previewUrl: "products.html#youtube-addon"
    },
    {
      id: "presentation",
      title: "Presentations",
      price: 30,
      previewUrl: "products.html#presentation"
    },
    {
      id: "banner",
      title: "Banner",
      price: 35,
      previewUrl: "products.html#banner"
    },
    {
      id: "menu",
      title: "Menus",
      price: 20,
      previewUrl: "products.html#menu"
    },
    {
      id: "celebration-cards",
      title: "Celebration cards",
      price: 10,
      previewUrl: "products.html#celebration-cards"
    }
    // Add more as needed...
  ];

  // ---- Cart logic ----
  function getCart() {
    return JSON.parse(localStorage.getItem('rytCart') || "[]");
  }
  function saveCart(cart) {
    localStorage.setItem('rytCart', JSON.stringify(cart));
  }
  function findProduct(idOrTitle) {
    return products.find(p => p.id === idOrTitle || p.title.toLowerCase() === idOrTitle.toLowerCase());
  }
  function addToCart(prodId) {
    let cart = getCart();
    let prod = findProduct(prodId);
    if (!prod) return;
    let idx = cart.findIndex(item => item.id === prodId);
    if (idx > -1) cart[idx].qty += 1;
    else cart.push({ id: prodId, title: prod.title, price: prod.price, qty: 1 });
    saveCart(cart);
    showNotif(`${prod.title} added to cart!`);
    renderCart();
  }
  function removeFromCart(idx) {
    let cart = getCart();
    cart.splice(idx, 1);
    saveCart(cart);
    renderCart();
  }
  function renderCart() {
    const cart = getCart();
    const cartList = document.getElementById('cartList');
    const cartTotal = document.getElementById('cartTotal');
    cartList.innerHTML = "";
    let total = 0;
    cart.forEach((item, idx) => {
      total += item.qty * item.price;
      cartList.innerHTML += `
        <li class="cart-item-box">
          <span class="cart-item-desc">${item.title} x ${item.qty} – $${item.qty * item.price}</span>
          <button class="cart-item-remove" onclick="removeFromCart(${idx})">Remove</button>
        </li>`;
    });
    cartTotal.textContent = "$" + total;
    if (cart.length === 0) {
      cartList.innerHTML = "<li style='color:#bbb; font-size:1.1em; padding:.8em 0;'>Cart is empty</li>";
    }
  }
  function onCheckout() {
    showNotif("Checkout is disabled in demo. (Implement as needed!)");
  }
  //---- Notification -----
  function showNotif(msg) {
    let n = document.getElementById('cartNotif');
    n.textContent = msg;
    n.classList.add('show');
    setTimeout(() => n.classList.remove('show'), 1700);
  }

  // ---- Search logic ----
  function renderSearchResults(results) {
    const out = document.getElementById('searchResults');
    if (!results || results.length === 0) {
      out.innerHTML = "";
      return;
    }
    out.innerHTML = results.map(prod =>
      `<div class="result-card">
        <span class="result-title">${prod.title} - <span class="result-price">$${prod.price}</span></span>
        <div class="result-actions">
          <button class="buy-btn" onclick="buyAndNotify('${prod.id}')">Buy</button>
          <a class="preview-btn" href="${prod.previewUrl}" target="_blank">Preview</a>
        </div>
      </div>`
    ).join("");
  }

  function buyAndNotify(prodId) {
    addToCart(prodId);
  }

  function onSearch() {
    const term = document.getElementById('searchInput').value.trim().toLowerCase();
    if (!term) return;
    const found = products.filter(p => p.title.toLowerCase().includes(term));
    renderSearchResults(found);
  }
  function quickSearch(keyword) {
    document.getElementById('searchInput').value = keyword;
    onSearch();
  }
  // Pre-populate a popular result as in screenshot
  window.addEventListener('DOMContentLoaded', () => {
    renderCart();
    // Show "Logos for businesses" buy result by default
    renderSearchResults([products[0]]);
  });
</script>
</body>
</html>
