
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
  --header-footer-bg: #333333;
  --text-color: #000000;
  --inverse-text-color: #ffffff;
  --accent: #008080;
}
body {
  background-color: var(--primary-bg);
  color: var(--text-color);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
}
a {
  color: var(--accent);
  text-decoration: none;
}
header {
  background-color: var(--header-footer-bg);
  padding: 1rem;
  text-align: center;
  color: var(--inverse-text-color);
}
header h1 {font-size:2rem;}
.products-section {
  max-width: 1300px;
  margin: 2rem auto;
  padding: 1rem;
  background: var(--secondary-bg);
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.07);
}
.products-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
}
.product-card {
  background: var(--primary-bg);
  border-radius: 10px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  width: 255px;
  transition: transform 0.24s;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1rem 1rem 1.5rem 1rem;
  position: relative;
}
.product-card img {
  width: 210px; height:140px; object-fit: cover;
  border-radius: 7px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  margin-bottom: 1rem;
  background: #f1f1f1;
}
.product-card h3 {
  margin-bottom: 0.5rem;
  font-size: 1.15rem;
  color: var(--text-color);
  text-align: center;
  font-weight: 600;
}
.product-card p {
  font-size: 0.95rem;
  margin-bottom: 1rem;
  min-height: 28px;
  text-align: center;
  color: #333;
}
.product-price {
  font-size: 1.18rem;
  font-weight: bold;
  color: var(--accent);
  margin-bottom: 0.8rem;
}
.product-actions {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
  width: 100%;
  justify-content: center;
}
.product-actions button {
  padding: 0.6rem 1.2rem;
  border: none;
  color: var(--inverse-text-color);
  font-size: 0.97rem;
  font-weight: bold;
  cursor: pointer;
  border-radius: 4px;
  background-color: var(--accent);
  transition: background-color 0.2s, transform 0.2s;
}
.product-actions button.buy-btn {
  background: linear-gradient(45deg, var(--accent), darkcyan);
  box-shadow: 0 3px 8px rgba(0,0,0,0.15);
}
.product-actions button:hover {
  background: darkcyan;
  transform: translateY(-2px);
}
@media (max-width:900px){
  .products-grid { flex-direction: column; align-items:center;}
  .product-card { width: 95%; max-width: 310px;}
}
footer {
  margin-top:2rem;
  background-color: var(--header-footer-bg);
  text-align: center;
  padding: 1rem;
  color: var(--inverse-text-color);
}
footer a { color: var(--accent); text-decoration: none; font-weight: bold;}
footer a:hover { color: var(--inverse-text-color);}
.section-title {text-align:center; font-size:1.8rem; margin-bottom:2rem; letter-spacing:1px;}
/* Back to Home Button */
.back-home-btn {
  display:inline-block;
  padding:0.7rem 1.6rem;
  background:linear-gradient(45deg, var(--accent), darkcyan);
  color:var(--inverse-text-color);
  border:none;
  border-radius:5px;
  text-decoration:none;
  font-weight:600;
  font-size:1rem;
  transition:background 0.25s, transform 0.15s;
  margin: 1.5rem auto 0 auto;
  box-shadow:0 3px 10px rgba(0,0,0,0.13);
}
.back-home-btn:hover {
  background: darkcyan;
  color: var(--inverse-text-color);
  transform: translateY(-2px);
}
</style>
</head>
<body>
<header>
  <h1>Products - RYT DESIGNS</h1>
</header>

<!-- Back to Home Button -->
<div style="width:100%;text-align:center;margin:1.5rem 0 0 0;">
  <a class="back-home-btn" href="https://rytdesignsca.github.io/">&#8592; Back to Home</a>
</div>

<section class="products-section">
<div class="section-title">Our Products &amp; Services</div>
<div class="products-grid">

<!-- Poster / Flyer -->
<!-- Portfolio Images -->
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Album%20cover.png" alt="A A itinerary.png">
  <div class="caption">A A itinerary.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Product%20label.png" alt="Album cover.png">
  <div class="caption">Album cover.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Skin.png" alt="Banner 4 website.png">
  <div class="caption">Banner 4 website.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/T-Shirt%20design.png" alt="Logo 4 website.png">
  <div class="caption">Logo 4 website.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Designs%20Poster.png" alt="Menu 4 website.png">
  <div class="caption">Menu 4 website.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Product%20label.png" alt="Product label.png">
  <div class="caption">Product label.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Designs%20Poster.png" alt="Ryt Designs Poster.png">
  <div class="caption">Ryt Designs Poster.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Skin.png" alt="Ryt Skin.png">
  <div class="caption">Ryt Skin.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/T-Shirt%20design.png" alt="T-Shirt design.png">
  <div class="caption">T-Shirt design.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Album%20cover.png" alt="Business card proto.jpg">
  <div class="caption">Business card proto.jpg</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Product%20label.png" alt="Celeb 4 website.png">
  <div class="caption">Celeb 4 website.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Skin.png" alt="Invitation 4 website.png">
  <div class="caption">Invitation 4 website.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/T-Shirt%20design.png" alt="Product 4 website.jpg">
  <div class="caption">Product 4 website.jpg</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Designs%20Poster.png" alt="Ryt designs presentation.pdf">
  <div class="caption">Ryt designs presentation.pdf</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Product%20label.png" alt="Ryt designs video.mp4">
  <div class="caption">Ryt designs video.mp4</div>
  <div class="label">RYT DESIGNS</div>
</div>
<div class="portfolio-item">
  <img src="https://rytdesignsca.github.io/website%20prototype/Ryt%20Skin.png" alt="YouTube thumbnail 4 website.png">
  <div class="caption">YouTube thumbnail 4 website.png</div>
  <div class="label">RYT DESIGNS</div>
</div>
<!-- Other Items -->
<div class="product-card">
<img src="website prototype/Ryt Skin.png" alt="Ryt Skin" />
<h3>Ryt Skin</h3>
<p>Product or graphics related to the Ryt Skin collection.</p>
<div class="product-price">$25</div>
<div class="product-actions">
<button class="buy-btn" onclick="buyNow('Ryt Skin', 25)">Buy Now</button>
<button onclick="addToCart('Ryt Skin', 25)">Add to Cart</button>
</div>
</div>

<div class="product-card">
<img src="website prototype/T-Shirt design.png" alt="T-Shirt Design" />
<h3>T-Shirt Design</h3>
<p>Bold custom t-shirt graphics, both front and back!</p>
<div class="product-price">$22</div>
<div class="product-actions">
<button class="buy-btn" onclick="buyNow('T-Shirt Design', 22)">Buy Now</button>
<button onclick="addToCart('T-Shirt Design', 22)">Add to Cart</button>
</div>
</div>

<div class="product-card">
<img src="website prototype/Ryt Designs (new logo) (1).png" alt="New Logo" />
<h3>New Logo Version</h3>
<p>Alternative new look for your branding needs.</p>
<div class="product-price">$30</div>
<div class="product-actions">
<button class="buy-btn" onclick="buyNow('New Logo Version', 30)">Buy Now</button>
<button onclick="addToCart('New Logo Version', 30)">Add to Cart</button>
</div>
</div>

</div>
</section>

<footer>
<p>&copy; 2025 RYT DESIGNS. All Rights Reserved.</p>
<p>Designed by RYT DESIGNS</p>
<p><a href="index.html">Back to Home</a></p>
</footer>

<script>
let cart = [];
function addToCart(name, price) {
  const existing = cart.find(item => item.name === name);
  if (existing) {
    existing.quantity += 1;
  } else {
    cart.push({ name: name, price: price, quantity: 1 });
  }
  alert(name + " has been added to your cart.");
  console.log(cart);
}
function buyNow(name, price) {
  alert("Proceeding to buy " + name + " for $" + price + ".");
}
</script>
</body>
</html>
