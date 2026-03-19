# venkyyyy
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WebDev Pro Services</title>
    <link rel="stylesheet" href="style.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <h1>WebDev Pro</h1>
            <nav>
                <a href="#home">Home</a>
                <a href="#services">Services</a>
                <a href="#contact">Contact</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container hero-content">
            <h2>Modern Web Development</h2>
            <p>We create responsive, clean, and visually stunning websites that help your business grow online.</p>
            <a href="#contact" class="btn">Get in Touch</a>
        </div>
        <div class="hero-image">
            <img src="https://cdn.pixabay.com/photo/2017/08/05/11/16/computer-2587246_1280.png" alt="Web Development Graphic">
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <div class="container">
            <h2>Our Services</h2>
            <div class="service-cards">
                <div class="card">
                    <h3>Web Development</h3>
                    <p>We build responsive, modern, and fast websites tailored to your needs.</p>
                </div>
                <div class="card">
                    <h3>UI/UX Design</h3>
                    <p>Designing beautiful and user-friendly interfaces for your website and apps.</p>
                </div>
                <div class="card">
                    <h3>Website Maintenance</h3>
                    <p>Keep your website secure, updated, and running smoothly all the time.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Call or WhatsApp: <strong>8341796749</strong></p>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2026 WebDev Pro Services. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
style.css
/* General Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto', sans-serif;
}

body {
    line-height: 1.6;
    color: #333;
    background-color: #f5f7fa;
}

/* Container */
.container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
}

/* Header */
header {
    background: #fff;
    padding: 20px 0;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 100;
}

header h1 {
    display: inline-block;
    color: #007BFF;
}

header nav {
    float: right;
}

header nav a {
    margin-left: 20px;
    text-decoration: none;
    color: #333;
    font-weight: 500;
    transition: color 0.3s;
}

header nav a:hover {
    color: #007BFF;
}

/* Hero Section */
.hero {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    padding: 60px 0;
    background: linear-gradient(135deg, #6CC1FF, #3A8DFF);
    color: #fff;
}

.hero h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
    animation: slideIn 1s ease-out;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 30px;
    max-width: 500px;
}

.hero .btn {
    padding: 12px 30px;
    background: #fff;
    color: #3A8DFF;
    font-weight: bold;
    border-radius: 25px;
    text-decoration: none;
    transition: transform 0.3s;
}

.hero .btn:hover {
    transform: scale(1.1);
}

/* Hero Image */
.hero-image img {
    max-width: 400px;
    animation: float 3s ease-in-out infinite;
}

/* Services Section */
.services {
    padding: 80px 0;
    text-align: center;
}

.services h2 {
    margin-bottom: 50px;
    font-size: 2.2rem;
    color: #007BFF;
}

.service-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background: #fff;
    padding: 30px;
    border-radius: 15px;
    width: 300px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.card:hover {
    transform: translateY(-10px);
    box-shadow: 0 12px 30px rgba(0,0,0,0.2);
}

.card h3 {
    margin-bottom: 15px;
    color: #007BFF;
}

/* Contact Section */
.contact {
    padding: 80px 0;
    background: #007BFF;
    color: #fff;
    text-align: center;
}

.contact form {
    margin-top: 30px;
    max-width: 500px;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.contact input, .contact textarea {
    padding: 12px;
    border: none;
    border-radius: 8px;
}

.contact button {
    padding: 12px;
    border: none;
    border-radius: 25px;
    background: #fff;
    color: #007BFF;
    font-weight: bold;
    cursor: pointer;
    transition: transform 0.3s;
}

.contact button:hover {
    transform: scale(1.05);
}

/* Footer */
footer {
    text-align: center;
    padding: 20px 0;
    background: #333;
    color: #fff;
}

/* Animations */
@keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
}

@keyframes slideIn {
    from { transform: translateX(-50px); opacity: 0; }
    to { transform: translateX(0); opacity: 1; }
}

/* Responsive */
@media (max-width: 900px) {
    .hero {
        flex-direction: column-reverse;
        text-align: center;
    }

    .hero-image img {
        max-width: 300px;
        margin-bottom: 30px;
    }

    header nav {
        float: none;
        margin-top: 10px;
    }

    .service-cards {
        flex-direction: column;
        align-items: center;
    }
}
