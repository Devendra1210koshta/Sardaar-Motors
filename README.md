<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sardaar Motors | High-Tech Garage</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Orbitron', sans-serif;
    }

    body {
      background: #0a0a0a;
      color: #fff;
    }

    header {
      display: flex;
      justify-content: space-between;
      padding: 20px 50px;
      background: rgba(0,0,0,0.8);
      position: sticky;
      top: 0;
    }

    header h1 {
      color: #00f7ff;
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #fff;
      transition: 0.3s;
    }

    nav a:hover {
      color: #00f7ff;
    }

    .hero {
      height: 90vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.9)),
                  url('https://images.unsplash.com/photo-1503376780353-7e6692767b70') no-repeat center/cover;
    }

    .hero h2 {
      font-size: 3rem;
      color: #00f7ff;
    }

    .hero p {
      margin: 20px 0;
    }

    .btn {
      padding: 12px 25px;
      background: #00f7ff;
      border: none;
      color: #000;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn:hover {
      background: #fff;
    }

    section {
      padding: 60px 50px;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: #111;
      padding: 20px;
      border-radius: 10px;
      border: 1px solid #00f7ff;
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 15px #00f7ff;
    }

    .about {
      text-align: center;
    }

    .stats {
      display: flex;
      justify-content: space-around;
      margin-top: 30px;
    }

    .stats div {
      text-align: center;
    }

    .contact form {
      display: flex;
      flex-direction: column;
      max-width: 500px;
      margin: auto;
    }

    .contact input, .contact textarea {
      margin: 10px 0;
      padding: 10px;
      border: none;
      outline: none;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #000;
      color: #888;
    }
  </style>
</head>

<body>

<header>
  <h1>Sardaar Motors</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero" id="home">
  <div>
    <h2>High-Tech Garage Solutions</h2>
    <p>Advanced Car Diagnostics | Performance Tuning | Premium Care</p>
    <button class="btn" onclick="scrollToSection('contact')">Book Service</button>
  </div>
</section>

<section id="services">
  <h2>Our Services</h2>
  <div class="services">
    <div class="card">
      <h3>AI Diagnostics</h3>
      <p>Smart car scanning and fault detection.</p>
    </div>
    <div class="card">
      <h3>Engine Tuning</h3>
      <p>Boost performance with advanced tuning tools.</p>
    </div>
    <div class="card">
      <h3>diesel engine and petrol engine Vehicle Repair</h3>
      <p>Specialized EV servicing and battery care.</p>
    </div>
    <div class="card">
      <h3>Custom Modifications</h3>
      <p>Upgrade your car with premium modifications.</p>
    </div>
  </div>
</section>

<section class="about" id="about">
  <h2>About Sardaar Motors</h2>
  <p>We are a futuristic garage delivering cutting-edge automotive solutions with precision and innovation.</p>

  <div class="stats">
    <div>
      <h3>5000+</h3>
      <p>Cars Serviced</p>
    </div>
    <div>
      <h3>10+</h3>
      <p>Years Experience</p>
    </div>
    <div>
      <h3>100%</h3>
      <p>Customer Satisfaction</p>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <h2>book your first car service</h2>
  <form onsubmit="submitForm(event)">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <input type="phone no" placeholder="phone no" required>
    <input type="model" placeholder="model" required>
    <textarea placeholder="Your Message"></textarea>
    <button class="btn">Send Message</button>
  </form>
</section>

<footer>
  <p>© 2026 Sardaar Motors | All Rights Reserved</p>
</footer>

<script>
  function scrollToSection(id) {
    document.getElementById(id).scrollIntoView({ behavior: 'smooth' });
  }

  function submitForm(e) {
    e.preventDefault();
    alert("Thank you! We will contact you soon.");
  }
</script>

</body>
</html>
