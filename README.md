<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Nairobi Comfort Cate - Experience luxury and comfort at its best.">
    <title>Nairobi Comfort Cate</title>
    <link rel="stylesheet" href="styles.css">
    <!-- Google Fonts for a modern feel -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Header with navigation -->
    <header>
        <div class="logo">
            <h1>Nairobi Comfort Cate</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h2>Welcome to Nairobi Comfort Cate</h2>
            <p>Your ultimate escape in Nairobi. Experience comfort like never before.</p>
            <a href="#contact" class="cta-button">Book Your Stay</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <div class="about-text">
                <h2>About Us</h2>
                <p>At Nairobi Comfort Cate, we provide world-class accommodations with personalized services. Whether you're here for business or leisure, we ensure your experience is nothing less than extraordinary.</p>
            </div>
            <div class="about-image">
                <img src="your_image_path.jpg" alt="Comfortable Room">
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-container">
            <div class="service-item">
                <i class="service-icon fas fa-bed"></i>
                <h3>Luxury Rooms</h3>
                <p>Relax in our spacious, elegantly furnished rooms designed for maximum comfort.</p>
            </div>
            <div class="service-item">
                <i class="service-icon fas fa-concierge-bell"></i>
                <h3>24/7 Concierge</h3>
                <p>Our dedicated concierge service is available around the clock to cater to your needs.</p>
            </div>
            <div class="service-item">
                <i class="service-icon fas fa-utensils"></i>
                <h3>Fine Dining</h3>
                <p>Indulge in world-class dining with a variety of local and international cuisines.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <form action="#" method="POST">
            <label for="name">Your Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Your Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Message:</label>
            <textarea id="message" name="message" rows="4" required></textarea>

            <button type="submit">Submit</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-container">
            <div class="footer-logo">
                <h1>Nairobi Comfort Cate</h1>
            </div>
            <div class="footer-nav">
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
            <p>&copy; 2025 Nairobi Comfort Cate. All Rights Reserved.</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
