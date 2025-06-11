
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="description" content="Product & Portfolio - RYT DESIGNS" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>RYT DESIGNS Products & Portfolio</title>
<style>
:root {
  --primary-bg: #ffffff;
  --secondary-bg: #f7f7f7;
  --header-footer-bg: #333333;
  --text-color: #000000;
  --inverse-text-color: #fff;
  --accent: #008080;
}
* {margin:0; padding:0; box-sizing:border-box;}
body {
  background: var(--primary-bg);
  color: var(--text-color);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
}
header {
  background: var(--header-footer-bg);
  text-align: center;
  padding: 1.2rem 0 0.5rem 0;
  color: var(--inverse-text-color);
}
h1 {font-size:2rem;}
a {
  color: var(--accent);
  text-decoration: none;
}
.cart-section {
  max-width: 800px;
  margin: 2rem auto 1.5rem auto;
  padding: 1.2rem 1rem 1.2rem 1rem;
  background: var(--secondary-bg);
  border-radius: 18px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.06);
}
.cart-title {
  font-size:1.25rem;
  font-weight: 700;
  margin-bottom: 1rem;
  color: var(--accent);
}
.cart-list {
  list-style: none;
  margin-bottom: 0.6rem;
}
.cart-list li {
  padding: 0.4rem 0;
  font-size: 1rem;
}
.cart-total {
  font-weight: 600;
  color: var(--header-footer-bg);
}
.clear-cart-btn {
  background: #ee6666;
  color: #fff;
  border: none;
  border-radius: 6px;
  padding: 0.4rem 1rem;
  cursor: pointer;
  font-weight: 600;
  font-size: 0.98rem;
  margin-top: 0.5rem;
}

.back-home-btn {
  display:inline-block;
  padding:0.7rem 1.6rem;
  background:linear-gradient(45deg, var(--accent), darkcyan);
  color:var(--inverse-text-color);
  border:none;
  border-radius:7px;
  text-decoration:none;
  font-weight:600;
  font-size:1rem;
  transition:background 0.25s, transform 0.15s;
  margin: 1.2rem auto 0 auto;
  box-shadow:0 3px 10px rgba(0,0,0,0.13);
}
.back-home-btn:hover {
  background: darkcyan;
  color: var(--inverse-text-color);
  transform: translateY(-2px);
}

.section-title {
  text-align:center; 
  font-size:1.6rem; 
  margin:2.5rem 0 1.5rem 0; 
  letter-spacing:1px; 
  color: var(--accent);
  font-weight: 700;
}
.products-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.4rem;
  max-width: 1300px;
  margin: auto;
  margin-bottom: 2rem;
}
.product-card {
  background: var(--primary-bg);
  border-radius: 17px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.055);
  padding: 1.1rem 1rem 1.5rem 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: transform 0.18s;
  min-height: 292px;
}
.product-card:hover {
  transform:scale(1.027) translateY(-5px);
  box-shadow: 0 6px 20px rgba(0,0,0,0.13);
}
.product-card img {
  width: 170px;
  height: 120px;
  object-fit: cover;
  border-radius: 12px;
  background: #f3f3f3;
  margin-bottom: 1rem;
}
.product-desc {
  font-size: 0.97rem;
  color: #333;
  text-align: center;
  margin-bottom: 0.4rem;
  min-height: 35px;
}
.product-name {
  font-size: 1.08rem;
  font-weight: 700;
  color: var(--header-footer-bg);
  margin-bottom: 0.2rem;
  letter-spacing:0.2px;
}
.buy-btn, .add-cart-btn {
  padding: 0.68rem 1.13rem;
  border: none;
  color: var(--inverse-text-color);
  font-size: 0.99rem;
  font-weight: bold;
  cursor: pointer;
  border-radius: 6px;
  margin-top: 0.6rem;
  background: linear-gradient(45deg, var(--accent), darkcyan);
  box-shadow: 0 2px 5px rgba(0,0,0,0.08);
  transition: background 0.18s, transform 0.11s;
}
.buy-btn:hover, .add-cart-btn:hover {
  background: darkcyan;
  transform: translateY(-1.7px) scale(1.025);
}
@media (max-width:1100px) {
  .products-grid { grid-template-columns: 1fr 1fr 1fr; }
}
@media (max-width: 850px) {
  .products-grid { grid-template-columns: 1fr 1fr;}
}
@media (max-width:550px) {
  .products-grid { grid-template-columns: 1fr;}
}
footer {
  margin-top:2rem;
  background: var(--header-footer-bg);
  color: var(--inverse-text-color);
  text-align: center;
  padding: 1.2rem 1rem 1.3rem 1rem;
  border-radius: 7px 7px 0 0;
}
footer a { color: var(--accent); text-decoration: none; font-weight: bold;}
footer a:hover { color: var(--inverse-text-color);}
.menu {
  text-align: center;
  margin: 1rem 0 0.7rem 0;
}
.menu a {
  display: inline-block;
  padding: 0.5rem 1.2rem;
  margin: 1px 0.4rem;
  border-radius: 5px;
  font-weight: 600;
  color: var(--accent);
  background: #f1f1f1;
}
.menu a:hover { background: var(--secondary-bg); color: darkcyan;}
</style>
</head>
<body>
<header>
  <h1>Products & Portfolio - RYT DESIGNS</h1>
</header>

<!-- Example Navigation/Menu -->
<div class="menu">
  <a class="back-home-btn" href="https://rytdesignsca.github.io/">&#8592; Back to Home</a>
  <!-- Place the following link where you want users to go to Products page with cart transfer -->
  <a href="javascript:void(0)" onclick="transferCartToProducts(); closeMenu();">Products</a>
</div>

<!-- CART SECTION -->
<section class="cart-section" id="cart-section">
  <div class="cart-title">🛒 Your Cart</div>
  <ul class="cart-list" id="cart-list">
    <!-- Cart items inserted here -->
  </ul>
  <div class="cart-total" id="cart-total">Total: $0</div>
  <button class="clear-cart-btn" onclick="clearCart()">Clear Cart</button>
</section>

<!-- ALBUM COVER SECTION -->
<div class="section-title">Album Cover</div>
<div class="products-grid">
  <div class="product-card">
    <img src="https://rytdesignsca.github.io/website%20prototype/Album%20cover.png" alt="Album Cover">
    <div class="product-name">Album Cover</div>
    <div class="product-desc">Beautiful cover art for albums and singles.</div>
    <button class="buy-btn" onclick="buyNow('Album Cover', 20)">Buy Now - $20</button>
    <button class="add-cart-btn" onclick="addToCart('Album Cover', 20)">Add to Cart</button>
  </div>
</div>

<!-- BUSINESS LOGO SECTION -->
<div class="section-title">Business Logo</div>
<div class="products-grid">
  <div class="product-card">
    <img src="https://rytdesignsca.github.io/website%20prototype/Logo%204%20website.png" alt="Business Logo">
    <div class="product-name">Business Logo</div>
    <div class="product-desc">Professional custom logo design for your business.</div>
    <button class="buy-btn" onclick="buyNow('Business Logo', 30)">Buy Now - $30</button>
    <button class="add-cart-btn" onclick="addToCart('Business Logo', 30)">Add to Cart</button>
  </div>
</div>

<!-- PACKAGE LABEL SECTION -->
<div class="section-title">Package Label</div>
<div class="products-grid">
  <div class="product-card">
    <img src="https://rytdesignsca.github.io/website%20prototype/Product%20label.png" alt="Package Label">
    <div class="product-name">Package Label</div>
    <div class="product-desc">Attractive, informative product and package labeling.</div>
    <button class="buy-btn" onclick="buyNow('Package Label', 25)">Buy Now - $25</button>
    <button class="add-cart-btn" onclick="addToCart('Package Label', 25)">Add to Cart</button>
  </div>
</div>

<!-- T-SHIRT DESIGN SECTION -->
<div class="section-title">T-Shirt Design</div>
<div class="products-grid">
  <div class="product-card">
    <img src="https://rytdesignsca.github.io/website%20prototype/T-Shirt%20design.png" alt="T-Shirt Design">
    <div class="product-name">T-Shirt Design</div>
    <div class="product-desc">Custom t-shirt graphics, front and back!</div>
    <button class="buy-btn" onclick="buyNow('T-Shirt Design', 22)">Buy Now - $22</button>
    <button class="add-cart-btn" onclick="addToCart('T-Shirt Design', 22)">Add to Cart</button>
  </div>
</div>

<!-- BUSINESS FLYER SECTION -->
<div class="section-title">Business Flyer</div>
<div class="products-grid">
  <div class="product-card">
    <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Designs%20Poster.png" alt="Business Flyer">
    <div class="product-name">Business Flyer</div>
    <div class="product-desc">Custom flyers for events, business, or announcement.</div>
    <button class="buy-btn" onclick="buyNow('Business Flyer', 15)">Buy Now - $15</button>
    <button class="add-cart-btn" onclick="addToCart('Business Flyer', 15)">Add to Cart</button>
  </div>
</div>

<footer>
  <p>&copy; 2025 RYT DESIGNS. All Rights Reserved.</p>
  <p>Designed by RYT DESIGNS</p>
  <p><a href="https://rytdesignsca.github.io/">Back to Home</a></p>
</footer>

<script>
    // CART with sessionStorage and key 'rytCart'
    let cart = JSON.parse(sessionStorage.getItem('rytCart') || '[]');
    const cartList = document.getElementById('cart-list');
    const cartTotal = document.getElementById('cart-total');

    function renderCart() {
      cartList.innerHTML = '';
      let total = 0;
      if (cart.length === 0) {
        cartList.innerHTML = '<li>Your cart is empty.</li>';
      } else {
        cart.forEach(item => {
          total += item.price * item.quantity;
          const li = document.createElement('li');
          li.textContent = item.name + " x" + item.quantity + " - $" + (item.price * item.quantity);
          cartList.appendChild(li);
        });
      }
      cartTotal.textContent = "Total: $" + total;
      sessionStorage.setItem('rytCart', JSON.stringify(cart));
    }
    function addToCart(name, price) {
      const item = cart.find(i => i.name === name);
      if (item) {
        item.quantity += 1;
      } else {
        cart.push({ name, price, quantity: 1 });
      }
      renderCart();
      alert(name + " has been added to your cart.");
    }
    function clearCart() {
      cart = [];
      renderCart();
    }
    function buyNow(name, price) {
      alert(`Proceeding to buy ${name} for $${price}.`);
    }
    // Transfer cart to products (sample, customize as needed)
    function transferCartToProducts() {
      // This function could redirect or update another page or modal
      alert("Cart will be available on the products page!");
      // Example (navigate to /products.html or whatever page):
      // window.location.href = "/products.html";
    }
    function closeMenu() {
      // Close your nav menu if you use a sidebar/drawer, else you can skip this
    }
    window.onload = renderCart;
</script>
</body>
</html>
