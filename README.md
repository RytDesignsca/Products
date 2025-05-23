
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>RYT DESIGNS Product Marketplace</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Segoe+UI:700,400">
  <style>
:root {
  --market-bg: #fff;
  --header-footer-bg: #333;
  --primary: #008080;
  --shadow: 0 3px 24px #0002;
  --border: #ececec;
  --cta: #ff7200;
  --cta-dark: #e05d00;
  --danger: #fe384c;
  --brand: #6457d9;
  --success: #16B36B;
  --text-main: #232629;
  --secondary: #f7f7f7;
  --yellow: #ffbb34;
  --badge-local: #45b75a;
  --badge-summer: #f69c2f;
  --card-radius: 13px;
}
body {
  margin:0; padding:0; background:var(--secondary); color:var(--text-main);
  font-family:'Segoe UI',Tahoma,Geneva,Verdana,sans-serif; line-height:1.52;
}
header {
  padding: 1.7rem .6rem 1rem .6rem; text-align:center;
  background: var(--header-footer-bg); color: #fff; font-size:2.2em; letter-spacing:.6px;
}
.market-section-title {
  font-size:1.23rem;margin:2.1em 0 .95em 1.50em; font-weight: 600; color: var(--primary);
  letter-spacing: .1px;
}
.market-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px,1fr));
  gap: 30px 21px;
  width: 100%;background: #fff;
  border-radius: 20px 20px 0 0;
  box-shadow: var(--shadow);
  padding: 0 17px 10px 24px;
  max-width: 1300px;
  margin: 0 auto 28px auto;
}
.market-card {
  background:#fff;
  border-radius: var(--card-radius);
  box-shadow: 0 5px 24px #a5b6b629;
  display: flex; flex-direction:column;
  position:relative; padding:0 0 16px 0; border:1.3px solid var(--border);
  margin-bottom: 2px; transition: box-shadow .18s, transform .16s;
  min-height:364px;
}
.market-card:hover {
  box-shadow: 0 15px 37px #8cd6c629; transform: translateY(-5px) scale(1.025);
  z-index:5;
}
.card-img-wrap {
  width: 100%; height: 133px;
  border-top-left-radius: var(--card-radius);
  border-top-right-radius: var(--card-radius);
  background:#f4fcfe; position: relative;
  display:flex; align-items:center; justify-content:center;
  overflow: hidden;
}
.card-img-wrap img {
  width:100%;height:100%;object-fit:cover;display:block;}
.market-badge {
  position:absolute;padding:2px 11px;font-size:11.3px;font-weight:700;
  border-radius:6px;top:8px;left:8px;color:#fff;z-index:3;box-shadow:0 1.5px 9px #feefc321;opacity:.93}
.badge-summer {background:var(--badge-summer);}
.badge-local {background:var(--badge-local);left:81px;}
.market-prod-title {
  margin:9px 0 6.5px 0;font-size:1.07em;font-weight:700;padding:0 9px;min-height:37px;word-break:break-all;color:#34302f;}
.card-pricing-row {display:flex;align-items:center;gap:7px;font-size:1.10em;font-weight:600;margin:2px 0 0 0;padding:0 9px 0 9px;}
.price-cta {color: var(--cta);font-weight:bold;}
.old-price {color:#aaa;text-decoration:line-through;font-size:.97em;font-weight:400;margin-left:5px;}
.card-dot {width:5.4px;height:5.4px;background:#efe03f;border-radius:50%;display:inline-block;margin:0 7px;}
.sold-counter, .instocktag {color:#bb8b27;font-weight:500;font-size:.92em;}
.instocktag {color: var(--danger);}
.market-highlight {
  font-size: .94em; color:var(--success); font-weight:600; margin-top:6px; margin-left:12px;
}
.rating-row {
  margin: 6.5px 0 2px 12px; display:flex; gap:7px; align-items:center;
  color:#333; font-weight:500; font-size:.97em;
}
.rstar {color:#FDB304;font-weight:700;font-size:1.10em;}
.r-revcount {font-size: .92em; color:#67676b; padding-left: 2px;}
.brand-row {display:flex; align-items:center; gap:5px; margin:7px 0 0 14px;}
.starseller-badge {
  background:var(--brand);
  color: #fff;font-size:.89em;border-radius:5px;padding:1.5px 8px;letter-spacing:.01em;
  font-weight:700;box-shadow: 0 1.5px 6px #6657d91b;}
.brand-badge {
  background: #f6e99f;
  color: #a6920d;font-size:.92em;
  font-weight:600;border-radius:4.2px;padding:1.5px 6px; margin-left:2px;
  border:1.3px solid #ecd03e66;
}
.market-cart-btn {
  position:absolute;right:13px;bottom:16px;background:#fcfcfc;border-radius:50%;
  box-shadow:0 1px 8px #ddb12216;
  border:none;padding:11px;cursor:pointer;transition:box-shadow .13s;z-index:2;
}
.market-cart-btn:hover { box-shadow:0 2px 14px #e6b83b38; background:#fffdd9;}
.market-cart-btn img{width:24px;height:24px;}
/* Highlight tags */
.used-tag {
  font-size: .92em;
  color: #598edb;
  font-weight: 600;
  margin-left: 15px;
}
.good-tag {
  color: var(--success);
  font-weight: 700;
  font-size: .94em;
}
.highlight-tag {
  background: #e8f7ef;
  color: #166c47;
  font-size:.93em;
  border-radius:4px;
  padding:2.2px 8px;
  margin-left:7px;
}
@media (max-width: 900px){
  .market-grid {gap:16px 7px;padding-left:6px;}
  .card-img-wrap {height:94px;}
}
@media (max-width:650px){
  .market-section-title {margin-left:.5em;}
  .market-grid {padding-right:5px;}
}
.cart-notif {
  position: fixed;
  left: 50%;
  top: 48px;
  z-index: 1500;
  background: var(--primary);
  color: #fff;
  border-radius: 16px;
  box-shadow: 0 3px 24px #2727ef25;
  font-weight:600;
  padding: 13px 33px;
  opacity: 0;
  pointer-events: none;
  font-size: 1.06em;
  transition: opacity 0.16s, transform 0.20s;
  transform: translateX(-50%) scale(.92);
}
.cart-notif.show { opacity: 1; pointer-events: all; transform: translateX(-50%) scale(1);}
  </style>
</head>
<body>
<header>
  RYT DESIGNS — Product Marketplace
</header>
<section>
  <div class="market-section-title">Items you may want to add</div>
  <div class="market-grid">
    <!-- Product Example 1 -->
    <div class="market-card">
      <div class="card-img-wrap">
        <img src="rytdesignsca-products-page/website/Album cover.png" alt="Album Cover" loading="lazy" />
        <span class="market-badge badge-summer">SUMMER</span>
        <span class="market-badge badge-local">Local</span>
      </div>
      <div class="market-prod-title">Album Cover - TUIKYO Wireless</div>
      <div class="card-pricing-row">
        <span class="price-cta">CA$21.49</span>
        <span class="old-price">45.99</span>
        <span class="card-dot"></span>
        <span class="sold-counter">931 sold</span>
      </div>
      <div class="market-highlight">CA$0.30 cheaper than viewed</div>
      <div class="rating-row">
        <span class="rstar">★</span> 4.6
        <span class="r-revcount">212</span>
      </div>
      <div class="brand-row">
        <span class="starseller-badge">★ Star seller</span>
        <span class="brand-badge">Brand: TUINYO</span>
      </div>
      <button class="market-cart-btn" onclick="addToCart('Album Cover - TUIKYO Wireless', 21.49)">
        <img src="https://img.icons8.com/material-outlined/24/000000/shopping-cart--v2.png" alt="cart" />
      </button>
    </div>
    <!-- Product Example 2 -->
    <div class="market-card">
      <div class="card-img-wrap">
        <img src="rytdesignsca-products-page/website/Banner 4 website.png" alt="Men's Stylish Two-Piece Hoodie" loading="lazy"/>
        <span class="market-badge badge-summer">SUMMER</span>
        <span class="market-badge badge-local">Local</span>
      </div>
      <div class="market-prod-title">Men's Stylish Two-Piece Hoodie</div>
      <div class="card-pricing-row">
        <span class="price-cta">CA$19.79</span>
        <span class="old-price">36.90</span>
        <span class="card-dot"></span>
        <span class="sold-counter">27K+ sold</span>
      </div>
      <div class="market-highlight">Lowest price in 30 days</div>
      <div class="rating-row">
        <span class="rstar">★</span> 4.8
        <span class="r-revcount">1,498</span>
      </div>
    </div>
    <!-- Product Example 3 -->
    <div class="market-card">
      <div class="card-img-wrap">
        <img src="rytdesignsca-products-page/website/youtube thumbnail 4 website.png" alt="Unisex Ski Cap" loading="lazy"/>
        <span class="market-badge badge-local">Local</span>
      </div>
      <div class="market-prod-title">2pcs Unisex Ski Cap Set</div>
      <div class="card-pricing-row">
        <span class="price-cta">CA$7.12</span>
        <span class="old-price">12.80</span>
        <span class="card-dot"></span>
        <span class="sold-counter">6.8K+ sold</span>
      </div>
      <div class="market-highlight">Lowest price in half year</div>
      <div class="rating-row">
        <span class="rstar">★</span> 4.6
        <span class="r-revcount">55</span>
      </div>
    </div>
    <!-- Example with only rating/brand -->
    <div class="market-card">
      <div class="card-img-wrap">
        <img src="rytdesignsca-products-page/website/Logo 4 website.png" alt="360 Rotatable Jewelry" loading="lazy"/>
        <span class="market-badge badge-local">Local</span>
      </div>
      <div class="market-prod-title">SOGES 360° Rotatable Jewelry Organizer</div>
      <div class="card-pricing-row">
        <span class="price-cta">CA$202.85</span>
        <span class="old-price"></span>
        <span class="card-dot"></span>
        <span class="sold-counter">102 sold</span>
      </div>
      <div class="rating-row">
        <span class="rstar">★</span> 4.9
        <span class="r-revcount">327</span>
      </div>
      <div class="brand-row">
        <span class="starseller-badge">★ Star seller</span>
        <span class="brand-badge">Brand: SOGES</span>
      </div>
    </div>
    <!-- Example with out-of-stock / limited info -->
    <div class="market-card">
      <div class="card-img-wrap">
        <img src="rytdesignsca-products-page/website/Menu 4 website.png" alt="Plush Slippers" loading="lazy"/>
      </div>
      <div class="market-prod-title">Cozy Plush Slip-On Slippers for Men</div>
      <div class="card-pricing-row">
        <span class="price-cta">CA$10.67</span>
        <span class="old-price">16.03</span>
        <span class="instocktag">ONLY 3 LEFT</span>
      </div>
      <div class="rating-row">
        <span class="rstar">★</span> 4.9
        <span class="r-revcount">97</span>
      </div>
    </div>
    <!-- Add more .market-card as needed, using the above styles -->
  </div>
</section>
<div class="cart-notif" id="cartNotif"></div>
<script>
  // Simple mock "cart"
  window.cart = [];
  function addToCart(name, price) {
    let cart = window.cart || [];
    let existing = cart.find(i=>i.name===name);
    if(existing) existing.quantity++;
    else cart.push({name, price, quantity:1});
    window.cart = cart;
    showNotif(name + " added to your cart!");
  }
  function showNotif(txt) {
    let n = document.getElementById('cartNotif');
    n.textContent = txt;
    n.classList.add('show');
    clearTimeout(window._cartnotiftimer);
    window._cartnotiftimer = setTimeout(()=>n.classList.remove('show'), 1550);
  }
</script>
</body>
</html>
