html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nairobi Comfort Care Service</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <div class="logo">
      <img src="logo.png" alt="Nairobi Comfort Care Service Logo">
    </div>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact Us</a></li>
      </ul>
    </nav>
  </header>

  <section id="home">
    <h1>Welcome to Nairobi Comfort Care Service</h1>
    <p>Providing compassionate and professional care for your loved ones.</p>
    <a href="#contact" class="cta-button">Book a Service</a>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>We are dedicated to improving the quality of life for our clients through personalized care.</p>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <ul>
      <li>in-Home Care</li>
      <li>Medical Assistance</li>
      <li>Elderly Care</li>
    </ul>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form action="submit_form.php" method="post">
      <input type="text" name="name" placeholder="KEVIN BIKETI RN"required>
      <input type="email" name="email" placeholder="sharuzbk11@gmail.com" required>
      <textarea name="message" placeholder="wecare while we serve" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>&copy; Nairobi Comfort Care Service. All rights reserved.</p>
  </footer>
</body>
</html>
