# Ma-Mobile-Accessories

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MA Mobile Accessories | Mobile Covers</title>
  <meta name="description" content="Shop stylish mobile covers at MA Mobile Accessories. Contact us on WhatsApp to order.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      background: #080808;
      color: white;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      width: 90%;
      max-width: 1150px;
      margin: auto;
    }

    header {
      background: #101010;
      border-bottom: 1px solid #292929;
      padding: 18px 0;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .navbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo {
      font-size: 23px;
      font-weight: bold;
    }

    .logo span,
    .red {
      color: #ed1c24;
    }

    nav {
      display: flex;
      gap: 22px;
    }

    nav a:hover {
      color: #ed1c24;
    }

    .btn {
      display: inline-block;
      background: #ed1c24;
      color: white;
      padding: 12px 20px;
      border-radius: 5px;
      border: none;
      cursor: pointer;
      font-weight: bold;
    }

    .btn:hover {
      background: #c90008;
    }

    /* Hero slider */

    .hero {
      min-height: 550px;
      display: flex;
      align-items: center;
      position: relative;
      overflow: hidden;
      background: #111;
    }

    .slide {
      position: absolute;
      inset: 0;
      background-size: cover;
      background-position: center;
      opacity: 0;
      transition: opacity 1s;
    }

    .slide.active {
      opacity: 1;
    }

    .hero::after {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(
        90deg,
        rgba(0,0,0,.94),
        rgba(0,0,0,.65),
        rgba(0,0,0,.15)
      );
    }

    .hero-content {
      position: relative;
      z-index: 2;
      max-width: 650px;
      padding: 90px 0;
    }

    .eyebrow {
      color: #ed1c24;
      font-weight: bold;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    h1 {
      font-size: clamp(38px, 6vw, 65px);
      line-height: 1.15;
      margin: 15px 0;
    }

    .hero p {
      color: #ddd;
      font-size: 17px;
      margin-bottom: 25px;
    }

    .dots {
      position: absolute;
      z-index: 3;
      bottom: 25px;
      left: 5%;
      display: flex;
      gap: 10px;
    }

    .dot {
      height: 12px;
      width: 12px;
      border: none;
      border-radius: 50%;
      background: #888;
      cursor: pointer;
    }

    .dot.active {
      background: #ed1c24;
    }

    /* Benefits */

    .benefits {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
      background: #141414;
      padding: 30px 5%;
      text-align: center;
    }

    .benefits h3 {
      font-size: 16px;
    }

    .benefits p {
      font-size: 13px;
      color: #aaa;
    }

    /* Products */

    section.content-section {
      padding: 75px 0;
    }

    .section-title {
      text-align: center;
      margin-bottom: 35px;
    }

    .section-title h2 {
      font-size: clamp(28px, 4vw, 40px);
      margin: 8px 0;
    }

    .section-title p {
      color: #aaa;
    }

    .product-tools {
      display: flex;
      gap: 15px;
      margin-bottom: 25px;
    }

    .product-tools input,
    .product-tools select {
      padding: 12px;
      background: #151515;
      color: white;
      border: 1px solid #333;
      border-radius: 5px;
    }

    .product-tools input {
      flex: 1;
      min-width: 0;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .product-card {
      background: #141414;
      border: 1px solid #292929;
      border-radius: 8px;
      overflow: hidden;
      transition: .3s;
    }

    .product-card:hover {
      transform: translateY(-5px);
      border-color: #ed1c24;
    }

    .product-card img {
      width: 100%;
      height: 270px;
      object-fit: cover;
      background: #222;
    }

    .product-info {
      padding: 20px;
    }

    .product-info h3 {
      margin: 5px 0;
    }

    .category {
      color: #ed1c24;
      font-size: 12px;
      text-transform: uppercase;
      font-weight: bold;
    }

    .description {
      color: #aaa;
      font-size: 14px;
      min-height: 45px;
    }

    .price {
      font-size: 21px;
      font-weight: bold;
      margin: 12px 0;
    }

    .product-buttons {
      display: flex;
      gap: 8px;
    }

    .product-buttons button {
      flex: 1;
      font-size: 13px;
      padding: 10px 5px;
    }

    .btn-outline {
      background: transparent;
      border: 1px solid #ed1c24;
    }

    /* About */

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 45px;
      align-items: center;
    }

    .about-grid img {
      width: 100%;
      height: 400px;
      object-fit: cover;
      border-radius: 8px;
    }

    .about-grid h2 {
      font-size: 36px;
      line-height: 1.2;
      margin: 12px 0;
    }

    .about-grid p {
      color: #bbb;
      margin-bottom: 20px;
    }

    .about-grid ul {
      list-style: none;
      margin-bottom: 25px;
    }

    .about-grid li {
      margin: 10px 0;
    }

    .about-grid li::before {
      content: "✓ ";
      color: #ed1c24;
      font-weight: bold;
    }

    /* CTA and FAQ */

    .cta {
      background: #21090a;
      border: 1px solid #521115;
      border-radius: 10px;
      text-align: center;
      padding: 45px 20px;
    }

    .cta h2 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    .cta p {
      color: #ccc;
      margin-bottom: 22px;
    }

    .faq-list {
      max-width: 800px;
      margin: auto;
    }

    details {
      background: #141414;
      border: 1px solid #292929;
      padding: 18px;
      margin: 12px 0;
      border-radius: 6px;
    }

    summary {
      cursor: pointer;
      font-weight: bold;
    }

    details p {
      color: #aaa;
      margin-top: 12px;
    }

    /* Contact */

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 25px;
    }

    .contact-box {
      background: #141414;
      padding: 25px;
      border: 1px solid #292929;
      border-radius: 8px;
    }

    .contact-box p {
      color: #bbb;
      margin: 12px 0;
    }

    .contact-form {
      display: grid;
      gap: 14px;
    }

    .contact-form input,
    .contact-form textarea {
      width: 100%;
      background: #080808;
      color: white;
      border: 1px solid #333;
      padding: 13px;
      border-radius: 5px;
      font: inherit;
    }

    .contact-form textarea {
      min-height: 120px;
      resize: vertical;
    }

    /* Footer */

    footer {
      background: #050505;
      border-top: 1px solid #292929;
      padding: 35px 0 20px;
      text-align: center;
    }

    footer p {
      color: #999;
      margin: 8px 0;
    }

    .footer-links {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      margin: 20px 0;
    }

    .footer-links a:hover {
      color: #ed1c24;
    }

    .whatsapp-float {
      position: fixed;
      right: 20px;
      bottom: 20px;
      z-index: 20;
      background: #25d366;
      color: #06190c;
      padding: 13px 18px;
      border-radius: 30px;
      font-weight: bold;
      box-shadow: 0 4px 15px #0008;
    }

    /* Cart */

    .cart-overlay {
      display: none;
      position: fixed;
      inset: 0;
      background: #000b;
      z-index: 100;
    }

    .cart-overlay.open {
      display: block;
    }

    .cart-panel {
      background: #111;
      width: min(420px, 100%);
      height: 100%;
      margin-left: auto;
      padding: 25px;
      display: flex;
      flex-direction: column;
    }

    .cart-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 20px;
    }

    .close-cart {
      background: none;
      color: white;
      border: none;
      font-size: 30px;
      cursor: pointer;
    }

    #cartItems {
      flex: 1;
      overflow-y: auto;
    }

    .cart-item {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      padding: 14px 0;
      border-bottom: 1px solid #333;
    }

    .cart-item button {
      color: #ed1c24;
      background: none;
      border: none;
      cursor: pointer;
    }

    .cart-total {
      padding-top: 20px;
    }

    .cart-total p {
      font-size: 20px;
      margin-bottom: 15px;
    }

    .cart-total button {
      width: 100%;
    }

    @media (max-width: 800px) {
      .navbar {
        flex-wrap: wrap;
      }

      nav {
        order: 3;
        width: 100%;
        justify-content: center;
        flex-wrap: wrap;
        gap: 14px;
      }

      .benefits {
        grid-template-columns: repeat(2, 1fr);
      }

      .product-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 520px) {
      .logo {
        font-size: 18px;
      }

      .hero {
        min-height: 490px;
      }

      .hero-content {
        padding: 70px 0;
      }

      .product-grid {
        grid-template-columns: 1fr;
      }

      .product-tools {
        flex-direction: column;
      }

      .product-tools input,
      .product-tools select {
        width: 100%;
      }

      .about-grid img {
        height: 280px;
      }

      .about-grid h2 {
        font-size: 30px;
      }

      .cta h2 {
        font-size: 26px;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="container navbar">
      <a href="#home" class="logo">MA <span>Mobile Accessories</span></a>

      <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#faq">FAQs</a>
        <a href="#contact">Contact</a>
      </nav>

      <button class="btn" id="openCart">
        Cart (<span id="cartCount">0</span>)
      </button>
    </div>
  </header>

  <main>

    <section class="hero" id="home">
      <div class="slide active" style="background-image:url('https://casebelle.co/cdn/shop/files/iphone-15-case-leather-obsidian-black-cb8.jpg?v=1764194561&width=1024')"></div>

      <div class="slide" style="background-image:url('https://coverscartonline.com/cdn/shop/collections/rn-image_picker_lib_temp_e3e72d23-5b5b-4cb0-a467-0a504ae1e16d.png?v=1778348676&width=1000')"></div>

      <div class="slide" style="background-image:url('https://img.zoreaksesuar.com/apple-iphone-15-plus-case-carbon-fiber-benks-essential-armorair-600d-kevlar-cover-with-magsafe-iphone-15-plus-benks-302815-28-B.jpg')"></div>

      <div class="container">
        <div class="hero-content">
          <span class="eyebrow">Style Meets Protection</span>
          <h1>Give Your Phone <span class="red">A Better Look.</span></h1>
          <p>Discover stylish mobile covers that add personality and everyday protection to your phone.</p>
          <a href="#products" class="btn">Explore Collection</a>
          <a href="#contact" class="btn btn-outline">Contact Us</a>
        </div>
      </div>

      <div class="dots">
        <button class="dot active" aria-label="Slide 1"></button>
        <button class="dot" aria-label="Slide 2"></button>
        <button class="dot" aria-label="Slide 3"></button>
      </div>
    </section>

    <section class="benefits">
      <div>
        <h3>◆ Stylish Designs</h3>
        <p>Modern phone styles</p>
      </div>
      <div>
        <h3>✓ Everyday Protection</h3>
        <p>Cases for daily use</p>
      </div>
      <div>
        <h3>♡ Great Choices</h3>
        <p>Different cover styles</p>
      </div>
      <div>
        <h3>↗ Easy Ordering</h3>
        <p>Order through WhatsApp</p>
      </div>
    </section>

    <section class="content-section" id="products">
      <div class="container">
        <div class="section-title">
          <span class="eyebrow">Our Collection</span>
          <h2>Find Your <span class="red">Perfect Cover</span></h2>
          <p>Explore our mobile cover collection.</p>
        </div>

        <div class="product-tools">
          <input id="search" type="search" placeholder="Search mobile covers...">

          <select id="category">
            <option value="all">All Categories</option>
            <option value="leather">Leather Covers</option>
            <option value="designer">Designer Covers</option>
            <option value="armor">Armor Covers</option>
            <option value="clear">Clear Covers</option>
          </select>
        </div>

        <div class="product-grid" id="productGrid">

          <article class="product-card" data-name="Black Leather Cover" data-category="leather" data-price="799">
            <img src="https://casebelle.co/cdn/shop/files/iphone-15-case-leather-obsidian-black-cb8.jpg?v=1764194561&width=1024" alt="Black leather mobile cover" loading="lazy">
            <div class="product-info">
              <span class="category">Leather Cover</span>
              <h3>Black Leather Cover</h3>
              <p class="description">Elegant and simple everyday style.</p>
              <p class="price">Rs. 799</p>
              <div class="product-buttons">
                <button class="btn btn-outline add">Add to Cart</button>
                <button class="btn order">Order Now</button>
              </div>
            </div>
          </article>

          <article class="product-card" data-name="Premium Designer Cover" data-category="designer" data-price="999">
            <img src="https://coverscartonline.com/cdn/shop/collections/rn-image_picker_lib_temp_e3e72d23-5b5b-4cb0-a467-0a504ae1e16d.png?v=1778348676&width=1000" alt="Designer mobile cover" loading="lazy">
            <div class="product-info">
              <span class="category">Designer Cover</span>
              <h3>Premium Designer Cover</h3>
              <p class="description">A fashionable look for your phone.</p>
              <p class="price">Rs. 999</p>
              <div class="product-buttons">
                <button class="btn btn-outline add">Add to Cart</button>
                <button class="btn order">Order Now</button>
              </div>
            </div>
          </article>

          <article class="product-card" data-name="Carbon Fiber Armor Cover" data-category="armor" data-price="1199">
            <img src="https://img.zoreaksesuar.com/apple-iphone-15-plus-case-carbon-fiber-benks-essential-armorair-600d-kevlar-cover-with-magsafe-iphone-15-plus-benks-302815-28-B.jpg" alt="Carbon fiber armor mobile cover" loading="lazy">
            <div class="product-info">
              <span class="category">Armor Cover</span>
              <h3>Carbon Fiber Armor Cover</h3>
              <p class="description">Modern textured premium design.</p>
              <p class="price">Rs. 1,199</p>
              <div class="product-buttons">
                <button class="btn btn-outline add">Add to Cart</button>
                <button class="btn order">Order Now</button>
              </div>
            </div>
          </article>

          <article class="product-card" data-name="Everyday Silicone Cover" data-category="designer" data-price="899">
            <img src="https://casebelle.co/cdn/shop/files/iphone-15-case-leather-obsidian-black-cb8.jpg?v=1764194561&width=1024" alt="Everyday mobile cover" loading="lazy">
            <div class="product-info">
              <span class="category">Silicone Cover</span>
              <h3>Everyday Silicone Cover</h3>
              <p class="description">Simple styling for everyday use.</p>
              <p class="price">Rs. 899</p>
              <div class="product-buttons">
                <button class="btn btn-outline add">Add to Cart</button>
                <button class="btn order">Order Now</button>
              </div>
            </div>
          </article>

          <article class="product-card" data-name="Transparent Clear Cover" data-category="clear" data-price="699">
            <img src="https://coverscartonline.com/cdn/shop/collections/rn-image_picker_lib_temp_e3e72d23-5b5b-4cb0-a467-0a504ae1e16d.png?v=1778348676&width=1000" alt="Clear mobile cover" loading="lazy">
            <div class="product-info">
              <span class="category">Clear Cover</span>
              <h3>Transparent Clear Cover</h3>
              <p class="description">Minimal style for your device.</p>
              <p class="price">Rs. 699</p>
              <div class="product-buttons">
                <button class="btn btn-outline add">Add to Cart</button>
                <button class="btn order">Order Now</button>
              </div>
            </div>
          </article>

          <article class="product-card" data-name="Premium Protection Cover" data-category="armor" data-price="1299">
            <img src="https://img.zoreaksesuar.com/apple-iphone-15-plus-case-carbon-fiber-benks-essential-armorair-600d-kevlar-cover-with-magsafe-iphone-15-plus-benks-302815-28-B.jpg" alt="Premium protective cover" loading="lazy">
            <div class="product-info">
              <span class="category">Armor Cover</span>
              <h3>Premium Protection Cover</h3>
              <p class="description">A bold, modern look for your phone.</p>
              <p class="price">Rs. 1,299</p>
              <div class="product-buttons">
                <button class="btn btn-outline add">Add to Cart</button>
                <button class="btn order">Order Now</button>
              </div>
            </div>
          </article>

        </div>
      </div>
    </section>

    <section class="content-section" id="about">
      <div class="container about-grid">
        <img src="https://casebelle.co/cdn/shop/files/iphone-15-case-leather-obsidian-black-cb8.jpg?v=1764194561&width=1024" alt="Mobile cover collection" loading="lazy">

        <div>
          <span class="eyebrow">About Our Store</span>
          <h2>Make Your Phone <span class="red">Stand Out.</span></h2>
          <p>Welcome to MA Mobile Accessories. Discover mobile covers that match your style and help personalize your everyday device.</p>
          <ul>
            <li>Different cover styles to explore</li>
            <li>Easy WhatsApp product enquiries</li>
            <li>Simple ordering process</li>
            <li>Friendly customer communication</li>
          </ul>
          <a href="#products" class="btn">Browse Products</a>
        </div>
      </div>
    </section>

    <section class="content-section">
      <div class="container">
        <div class="cta">
          <h2>Need Help Choosing a Cover?</h2>
          <p>Message us to ask about prices, phone models and availability.</p>
          <a class="btn whatsapp-link" href="#">Chat on WhatsApp</a>
        </div>
      </div>
    </section>

    <section class="content-section" id="faq">
      <div class="container">
        <div class="section-title">
          <span class="eyebrow">Got Questions?</span>
          <h2>Frequently Asked <span class="red">Questions</span></h2>
        </div>

        <div class="faq-list">
          <details>
            <summary>How can I order a mobile cover?</summary>
            <p>Click Order Now or add products to your cart and continue through WhatsApp.</p>
          </details>

          <details>
            <summary>Can I ask about my phone model?</summary>
            <p>Yes. Send us your phone brand and model on WhatsApp to ask about available covers.</p>
          </details>

          <details>
            <summary>Are these prices final?</summary>
            <p>These are sample prices. Confirm actual prices and delivery charges with us before ordering.</p>
          </details>

          <details>
            <summary>Can I order multiple products?</summary>
            <p>Yes. Add multiple products to your cart and send the order summary through WhatsApp.</p>
          </details>
        </div>
      </div>
    </section>

    <section class="content-section" id="contact">
      <div class="container">
        <div class="section-title">
          <span class="eyebrow">Get in Touch</span>
          <h2>Contact <span class="red">Us</span></h2>
          <p>Send us your questions or product enquiry.</p>
        </div>

        <div class="contact-grid">
          <div class="contact-box">
            <h3>MA Mobile Accessories</h3>
            <p>Ask about our mobile covers and available phone models.</p>
            <p><strong class="red">WhatsApp:</strong> 03244085090</p>
            <a href="#" class="btn whatsapp-link">Message Us</a>
          </div>

          <form class="contact-box contact-form" id="contactForm">
            <h3>Send an Enquiry</h3>
            <input id="customerName" type="text" placeholder="Your name" required>
            <input id="customerPhone" type="tel" placeholder="Your phone number" required>
            <input id="customerProduct" type="text" placeholder="Product or phone model">
            <textarea id="customerMessage" placeholder="Your message" required></textarea>
            <button type="submit" class="btn">Send via WhatsApp</button>
          </form>
        </div>
      </div>
    </section>

  </main>

  <footer>
    <div class="container">
      <a href="#home" class="logo">MA <span>Mobile Accessories</span></a>
      <p>Style your phone. Express yourself.</p>

      <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </div>

      <p>© <span id="year"></span> MA Mobile Accessories. All rights reserved.</p>
    </div>
  </footer>

  <a href="#" class="whatsapp-float whatsapp-link">WhatsApp</a>

  <!-- Cart drawer -->
  <div class="cart-overlay" id="cartOverlay">
    <aside class="cart-panel" role="dialog" aria-modal="true" aria-label="Shopping cart">
      <div class="cart-header">
        <h2>Your Cart</h2>
        <button class="close-cart" id="closeCart" aria-label="Close cart">×</button>
      </div>

      <div id="cartItems"></div>

      <div class="cart-total">
        <p>Total: <span id="cartTotal">Rs. 0</span></p>
        <button class="btn" id="checkoutButton">Checkout on WhatsApp</button>
      </div>
    </aside>
  </div>

  <script>
    // Your WhatsApp number in international format
    const WHATSAPP_NUMBER = "923244085090";

    function openWhatsApp(message) {
      const url = "https://wa.me/" + WHATSAPP_NUMBER +
        "?text=" + encodeURIComponent(message);

      window.open(url, "_blank", "noopener,noreferrer");
    }

    // WhatsApp links
    document.querySelectorAll(".whatsapp-link").forEach(link => {
      link.href = "https://wa.me/" + WHATSAPP_NUMBER +
        "?text=" + encodeURIComponent(
          "Hello MA Mobile Accessories! I want to ask about your products."
        );
      link.target = "_blank";
      link.rel = "noopener noreferrer";
    });

    // Automatic hero slider
    const slides = document.querySelectorAll(".slide");
    const dots = document.querySelectorAll(".dot");
    let currentSlide = 0;
    let sliderTimer;

    function showSlide(index) {
      slides.forEach((slide, i) =>
        slide.classList.toggle("active", i === index)
      );

      dots.forEach((dot, i) =>
        dot.classList.toggle("active", i === index)
      );

      currentSlide = index;
    }

    function startSlider() {
      clearInterval(sliderTimer);
      sliderTimer = setInterval(() => {
        showSlide((currentSlide + 1) % slides.length);
      }, 4500);
    }

    dots.forEach((dot, index) => {
      dot.addEventListener("click", () => {
        showSlide(index);
        startSlider();
      });
    });

    startSlider();

    // Product search and category filter
    const search = document.getElementById("search");
    const category = document.getElementById("category");
    const productGrid = document.getElementById("productGrid");
    const cards = document.querySelectorAll(".product-card");

    function filterProducts() {
      let visibleCount = 0;
      const query = search.value.toLowerCase().trim();

      cards.forEach(card => {
        const name = card.dataset.name.toLowerCase();
        const matchesSearch = name.includes(query);
        const matchesCategory =
          category.value === "all" ||
          card.dataset.category === category.value;

        const visible = matchesSearch && matchesCategory;
        card.style.display = visible ? "" : "none";

        if (visible) visibleCount++;
      });

      let emptyMessage = document.getElementById("emptyMessage");

      if (emptyMessage) emptyMessage.remove();

      if (visibleCount === 0) {
        emptyMessage = document.createElement("p");
        emptyMessage.id = "emptyMessage";
        emptyMessage.textContent = "No products found.";
        emptyMessage.style.cssText =
          "grid-column:1/-1;text-align:center;padding:25px;color:#aaa;";
        productGrid.appendChild(emptyMessage);
      }
    }

    search.addEventListener("input", filterProducts);
    category.addEventListener("change", filterProducts);

    // Product ordering
    cards.forEach(card => {
      card.querySelector(".order").addEventListener("click", () => {
        openWhatsApp(
          "Hello MA Mobile Accessories!\n\n" +
          "I want to order:\n" +
          "Product: " + card.dataset.name + "\n" +
          "Price: Rs. " +
          Number(card.dataset.price).toLocaleString("en-PK") +
          "\n\nPlease confirm availability and delivery charges."
        );
      });
    });

    // Shopping cart
    let cart = [];

    const cartOverlay = document.getElementById("cartOverlay");
    const cartItems = document.getElementById("cartItems");
    const cartCount = document.getElementById("cartCount");
    const cartTotal = document.getElementById("cartTotal");

    function money(amount) {
      return "Rs. " + amount.toLocaleString("en-PK");
    }

    function addToCart(name, price) {
      const existing = cart.find(item => item.name === name);

      if (existing) {
        existing.quantity++;
      } else {
        cart.push({ name, price, quantity: 1 });
      }

      renderCart();
    }

    function renderCart() {
      cartItems.innerHTML = "";

      cartCount.textContent = cart.reduce(
        (sum, item) => sum + item.quantity, 0
      );

      const total = cart.reduce(
        (sum, item) => sum + item.price * item.quantity, 0
      );

      cartTotal.textContent = money(total);

      if (cart.length === 0) {
        cartItems.textContent = "Your cart is empty.";
        cartItems.style.color = "#aaa";
        return;
      }

      cart.forEach(item => {
        const row = document.createElement("div");
        row.className = "cart-item";

        const details = document.createElement("div");
        const title = document.createElement("strong");
        title.textContent = item.name;

        const quantity = document.createElement("p");
        quantity.textContent =
          money(item.price) + " × " + item.quantity;

        details.append(title, quantity);

        const controls = document.createElement("div");
        const subtotal = document.createElement("strong");
        subtotal.textContent = money(item.price * item.quantity);

        const remove = document.createElement("button");
        remove.textContent = "Remove";
        remove.addEventListener("click", () => {
          cart = cart.filter(product => product.name !== item.name);
          renderCart();
        });

        controls.append(subtotal, document.createElement("br"), remove);
        row.append(details, controls);
        cartItems.appendChild(row);
      });
    }

    document.querySelectorAll(".add").forEach(button => {
      button.addEventListener("click", () => {
        const card = button.closest(".product-card");

        addToCart(
          card.dataset.name,
          Number(card.dataset.price)
        );

        const oldText = button.textContent;
        button.textContent = "Added!";
        setTimeout(() => button.textContent = oldText, 1000);
      });
    });

    document.getElementById("openCart").addEventListener("click", () => {
      cartOverlay.classList.add("open");
    });

    document.getElementById("closeCart").addEventListener("click", () => {
      cartOverlay.classList.remove("open");
    });

    cartOverlay.addEventListener("click", event => {
      if (event.target === cartOverlay) {
        cartOverlay.classList.remove("open");
      }
    });

    document.addEventListener("keydown", event => {
      if (event.key === "Escape") {
        cartOverlay.classList.remove("open");
      }
    });

    document.getElementById("checkoutButton").addEventListener("click", () => {
      if (cart.length === 0) {
        alert("Please add a product to your cart first.");
        return;
      }

      let message = "Hello MA Mobile Accessories!\nMy order:\n\n";

      cart.forEach((item, index) => {
        message += (index + 1) + ". " + item.name +
          "\nQuantity: " + item.quantity +
          "\nSubtotal: " + money(item.price * item.quantity) +
          "\n\n";
      });

      const total = cart.reduce(
        (sum, item) => sum + item.price * item.quantity, 0
      );

      message += "Total: " + money(total);
      message += "\nPlease confirm availability and delivery charges.";

      openWhatsApp(message);
    });

    // Contact form sends an enquiry to WhatsApp
    document.getElementById("contactForm").addEventListener("submit", event => {
      event.preventDefault();

      const name = document.getElementById("customerName").value.trim();
      const phone = document.getElementById("customerPhone").value.trim();
      const product = document.getElementById("customerProduct").value.trim();
      const message = document.getElementById("customerMessage").value.trim();

      openWhatsApp(
        "Hello MA Mobile Accessories!\n\n" +
        "Name: " + name + "\n" +
        "Customer phone: " + phone + "\n" +
        "Product / phone model: " + (product || "Not specified") + "\n" +
        "Message: " + message
      );
    });

    document.getElementById("year").textContent =
      new Date().getFullYear();

    renderCart();
  </script>

</body>
</html>
