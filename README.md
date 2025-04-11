<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="description" content="Product Page - RYT DESIGNS" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Product Page - RYT DESIGNS</title>
  <style>
    /* Global Styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

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

    /* Header */
    header {
      background-color: var(--header-footer-bg);
      padding: 1rem;
      text-align: center;
      color: var(--inverse-text-color);
    }

    header h1 {
      font-size: 2rem;
    }

    /* Product Section */
    .product-container {
      max-width: 1200px;
      margin: 2rem auto;
      padding: 1rem;
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
    }

    .product-image {
      flex: 1 1 400px;
      text-align: center;
    }

    .product-image img {
      max-width: 100%;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    .product-details {
      flex: 2 1 600px;
      padding: 1rem;
    }

    .product-details h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
    }

    .product-details p {
      margin-bottom: 1rem;
      font-size: 1.1rem;
    }

    .product-price {
      font-size: 1.5rem;
      font-weight: bold;
      color: var(--accent);
      margin-bottom: 1.5rem;
    }

    .product-actions {
      display: flex;
      gap: 1rem;
    }

    .product-actions button {
      padding: 0.75rem 1.5rem;
      background-color: var(--accent);
      border: none;
      color: var(--inverse-text-color);
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      border-radius: 4px;
      transition: background-color 0.3s ease;
    }

    .product-actions button:hover {
      background-color: darkcyan;
    }

    /* Related Products Section */
    .related-products {
      background-color: var(--secondary-bg);
      padding: 2rem;
    }

    .related-products h3 {
      text-align: center;
      margin-bottom: 2rem;
      font-size: 1.8rem;
    }

    .related-products-container {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
    }

    .related-product {
      background-color: var(--header-footer-bg);
      color: var(--inverse-text-color);
      padding: 1rem;
      border-radius: 8px;
      text-align: center;
      flex: 1 1 200px;
      transition: transform 0.3s ease;
    }

    .related-product:hover {
      transform: translateY(-5px);
    }

    .related-product img {
      max-width: 100%;
      border-radius: 4px;
      margin-bottom: 0.5rem;
    }

    .related-product h4 {
      margin-bottom: 0.5rem;
    }

    .related-product p {
      font-size: 0.9rem;
    }

    /* Footer */
    footer {
      background-color: var(--header-footer-bg);
      text-align: center;
      padding: 1rem;
      color: var(--inverse-text-color);
    }

    footer a {
      color: var(--accent);
      text-decoration: none;
      font-weight: bold;
    }

    footer a:hover {
      color: var(--inverse-text-color);
    }
  </style>
</head>
<body>
  <!-- Header -->
  <header>
    <h1>Product Page - RYT DESIGNS</h1>
  </header>

  <!-- Product Section -->
  <section class="product-container">
    <div class="product-image">
      <img src="website prototype/Logo 4 website.png" alt="Product Image" />
    </div>
    <div class="product-details">
      <h2>Logo Design</h2>
      <p>Our logo design service offers creative and professional designs tailored to your brand's identity.</p>
      <p>Stand out in the market with a memorable and impactful logo.</p>
      <div class="product-price">$30</div>
      <div class="product-actions">
        <button onclick="addToCart('Logo Design', 30)">Add to Cart</button>
        <button onclick="window.location.href='#contact'">Contact Us</button>
      </div>
    </div>
  </section>

  <!-- Related Products -->
  <section class="related-products">
    <h3>Related Products</h3>
    <div class="related-products-container">
      <div class="related-product">
        <img src="website prototype/business card proto.jpg" alt="Business Card" />
        <h4>Business Card Design</h4>
        <p>$20</p>
      </div>
      <div class="related-product">
        <img src="website prototype/invitation 4 website.png" alt="Invitation" />
        <h4>Invitation Design</h4>
        <p>$24</p>
      </div>
      <div class="related-product">
        <img src="website prototype/youtube thumbnail 4 website.png" alt="YouTube Thumbnail" />
        <h4>YouTube Thumbnail</h4>
        <p>$20</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 RYT DESIGNS. All Rights Reserved.</p>
    <p>Designed by RYT DESIGNS</p>
    <p><a href="index.html">Back to Home</a></p>
  </footer>

  <!-- JavaScript for Cart -->
  <script>
    let cart = [];
    function addToCart(name, price) {
      const existing = cart.find(item => item.name === name);
      if (existing) {
        existing.quantity += 1;
      } else {
        cart.push({ name, price, quantity: 1 });
      }
      alert(`${name} has been added to your cart.`);
      console.log(cart);
    }
  </script>
</body>
</html>
