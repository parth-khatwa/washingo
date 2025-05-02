# washingo
it is laundary tech platform which is providing laundary services
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>WashingO – We Believe in Quality</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    /* RESET & BASE */
    * { margin:0; padding:0; box-sizing:border-box; }
    body { font-family: 'Poppins', sans-serif; color:#333; background:#fff; }
    img { max-width:100%; display:block; }

    /* HEADER */
    .site-header {
      background:#ffd600; padding:1rem; text-align:center;
      display: flex; flex-direction: column; align-items: center;
    }
    .logo { height:100px; margin-bottom: 1rem; }
    .site-header h1 { font-size:2.2rem; margin:0.5rem; }
    .tagline { font-size:1.2rem; color:#555; }
    .site-nav a {
      margin:0 .8rem; text-decoration:none; color:#333; font-weight:600;
    }

    /* HERO */
    .hero {
      background: linear-gradient(135deg, #ffe082, #fff59d);
      padding:2rem; text-align:center;
    }
    .hero h2 { font-size:2.5rem; margin-bottom:1rem; }
    .hero p { margin-bottom:1.5rem; }
    .btn-primary {
      background:#2e7d32; color:#fff; padding:.8rem 1.5rem; border:none; border-radius:5px;
      text-decoration:none; font-weight:600; transition:opacity .2s;
    }
    .btn-primary:hover { opacity:.8; }

    /* SERVICES */
    .services { padding:2rem; text-align:center; }
    .services h2 { margin-bottom:1rem; font-size:1.8rem; }
    .grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(150px,1fr)); gap:1rem; }
    .card { background:#fafafa; padding:1rem; border-radius:8px; box-shadow:0 2px 6px rgba(0,0,0,.1); }
    .card h3 { margin-top:.5rem; }

    /* BOOKING */
    .booking { padding:2rem; background:#f1f8e9; text-align:center; }
    .booking h2 { margin-bottom:1rem; }
    .field { margin:1rem 0; text-align:left; }
    .field label { display:block; margin-bottom:.3rem; font-weight:600; }
    .field input, .field select {
      width:100%; padding:.6rem; border:1px solid #ccc; border-radius:5px;
    }
    .btn-secondary {
      background:#0277bd; color:#fff; padding:.6rem 1.2rem; border:none; border-radius:5px;
      cursor:pointer; transition:opacity .2s; font-weight:600;
    }
    .btn-secondary:hover { opacity:.8; }
    .response { margin-top:.8rem; font-weight:600; color:green; }

    /* PRICING */
    .pricing { padding:2rem; text-align:center; }
    .pricing table {
      width:80%; max-width:500px; margin:0 auto; border-collapse:collapse;
    }
    .pricing th, .pricing td {
      border:1px solid #ddd; padding:.8rem; font-weight:400;
    }
    .pricing th { background:#f5f5f5; }

    /* ABOUT & CONTACT */
    .about, .contact { padding:2rem; }
    .about h2, .contact h2 { margin-bottom:1rem; font-size:1.8rem; }
    .social img { width:32px; margin:.5rem; }

    /* FOOTER */
    .site-footer { text-align:center; padding:1rem; background:#e0e0e0; font-size:.9rem; }
  </style>
</head>
<body>
  <!-- Header Section -->
  <header class="site-header">
    <img src="washingO_logo.png" alt="WashingO Logo" class="logo">
    <h1>WashingO</h1>
    <p class="tagline">We believe in quality</p>
    <nav class="site-nav">
      <a href="#home">Home</a>
      <a href="#services">Services</a>
      <a href="#pricing">Pricing</a>
      <a href="#about">About Us</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section id="home" class="hero">
    <h2>Fastest Laundry Delivery in Dewas</h2>
    <p>Pickup &amp; Delivery • Dry Clean • Steam Press</p>
    <a href="#book" class="btn-primary">Book Your Laundry</a>
  </section>

  <!-- Services Section -->
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="grid">
      <div class="card">
        <img src="icon-wash.png" alt="Wash Icon">
        <h3>Normal Wash</h3>
      </div>
      <div class="card">
        <img src="icon-steam.png" alt="Steam Icon">
        <h3>Steam Press</h3>
      </div>
      <div class="card">
        <img src="icon-dry.png" alt="Dry Icon">
        <h3>Dry Clean</h3>
      </div>
      <div class="card">
        <img src="icon-lehenga.png" alt="Lehenga Icon">
        <h3>Lehenga Wash</h3>
      </div>
      <div class="card">
        <img src="icon-coat.png" alt="Coat Icon">
        <h3>Coat Wash</h3>
      </div>
    </div>
  </section>

  <!-- Booking Section -->
  <section id="book" class="booking">
    <h2>Place Your Laundry Order</h2>
    <form id="orderForm">
      <div class="field">
        <label>Clothing Type</label>
        <select name="clothes">
          <option>Shirt</option>
          <option>Pant</option>
          <option>Kurti</option>
          <option>Saree</option>
          <option>Lehenga</option>
          <option>Kurta Pajama</option>
          <option>Salwar Suit</option>
          <option>Coat</option>
        </select>
      </div>
      <div class="field">
        <label>Wash Type</label>
        <select name="washType">
          <option>Normal Wash</option>
          <option>Steam Press</option>
          <option>Dry Clean</option>
          <option>Lehenga Wash</option>
          <option>Coat Wash</option>
        </select>
      </div>
      <div class="field">
        <label>Pickup Date</label>
        <input type="date" name="pickupDate" required>
      </div>
      <div class="field">
        <label>Address</label>
        <input type="text" name="address" placeholder="Your pickup address" required>
      </div>
      <div class="field">
        <label>Mobile Number</label>
        <input type="tel" name="phone" pattern="[0-9]{10}" placeholder="10-digit number" required>
      </div>
      <button type="submit" class="btn-secondary">Place Order</button>
      <p id="responseMsg" class="response"></p>
    </form>
  </section>

  <!-- Pricing Section -->
  <section id="pricing" class="pricing">
    <h2>Pricing (Dewas)</h2>
    <table>
      <tr><th>Service</th><th>Rate</th></tr>
      <tr><td>Normal Wash (per kg)</td><td>₹60</td></tr>
      <tr><td>Wash & Iron (per kg)</td><td>₹80</td></tr>
      <tr><td>Dry Clean (per piece)</td><td>₹70</td></tr>
      <tr><td>Pickup & Delivery</td><td>Free (₹200+ bill)</td></tr>
    </table>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About WashingO</h2>
    <p>WashingO is your go-to laundry partner in Dewas (41). We connect you with expert washers, handle pickup & delivery, and ensure 30% tech-powered reliability. Founded by Parth Khatwa.</p>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <p>Email: contact@washingodewas.com • Phone: +91-XXXXXXXXXX</p>
    <div class="social">
      <a href="#"><img src="icon-insta.png" alt="Instagram"></a>
      <a href="#"><img src="icon-fb.png" alt="Facebook"></a>
    </div>
  </section>

  <!-- Footer Section -->
  <footer class="site-footer">
    &copy; 2025 WashingO by Parth Khatwa – All Rights Reserved
  </footer>

  <script>
    document.getElementById('orderForm').addEventListener('submit', async e => {
      e.preventDefault();
      const data = Object.fromEntries(new FormData(e.target));
      try {
        const res = await fetch('https://your-backend-url.com/api/book', {
          method: 'POST',
          headers: { 'Content-Type': 'application/json' },
          body: JSON.stringify(data)
        });
        const msg = await res.text();
        document.getElementById('responseMsg').textContent = msg;
      } catch (err) {
        document.getElementById('responseMsg').textContent = 'Error placing order.';
      }
    });
  </script>
</body>
</html>

