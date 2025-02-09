<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>University Landing Page</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        /* Navbar Styles */
        nav {
            background-color: #2C3E50;
            position: sticky;
            top: 0;
            z-index: 10;
            padding: 10px 20px;
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav .logo {
            font-size: 1.8rem;
            font-weight: bold;
        }

        nav ul {
            display: flex;
            gap: 20px;
            list-style-type: none;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
        }

        nav ul li a:hover {
            color: #3498db;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: url('https://hips.hearstapps.com/hbu.h-cdn.co/assets/17/32/980x480/gallery-1502296181-royal-roads-university.jpg?resize=1200:*') no-repeat center center/cover;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 30px;
        }

        .cta-button {
            padding: 15px 30px;
            background-color: #3498db;
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .cta-button:hover {
            background-color: #2980b9;
        }

        /* About Section */
        .about {
            padding: 60px 20px;
            text-align: center;
            background-color: #ecf0f1;
        }

        .about h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .about p {
            font-size: 1.2rem;
            max-width: 900px;
            margin: 0 auto 30px;
        }

        /* Programs Section */
        .programs {
            padding: 60px 20px;
            text-align: center;
        }

        .programs h2 {
            font-size: 2.5rem;
            margin-bottom: 30px;
        }

        .programs .programs-list {
            display: flex;
            justify-content: center;
            gap: 30px;
        }

        .programs .program {
            background-color: #fff;
            padding: 20px;
            width: 250px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .programs .program h3 {
            font-size: 1.6rem;
            margin-bottom: 15px;
        }

        .programs .program p {
            font-size: 1rem;
            margin-bottom: 15px;
        }

        /* Contact Section */
        .contact {
            padding: 60px 20px;
            text-align: center;
            background-color: #34495e;
            color: white;
        }

        .contact h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .contact p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        .contact a {
            padding: 10px 20px;
            background-color: #3498db;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }

        .contact a:hover {
            background-color: #2980b9;
        }

        /* Footer Section */
        footer {
            background-color: #2C3E50;
            padding: 30px 20px;
            color: white;
            text-align: center;
        }

        footer a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
        }

        footer a:hover {
            color: #3498db;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .programs .programs-list {
                flex-direction: column;
                gap: 20px;
            }

            .hero h1 {
                font-size: 3rem;
            }

            .hero p {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav>
        <div class="logo">RD University</div>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#programs">Programs</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <div class="hero">
        <div>
            <h1>Welcome to RD University</h1>
            <p>Your future starts here.</p>
            <a href="#contact" class="cta-button">Join Now</a>
        </div>
    </div>

    <!-- About Section -->
    <div id="about" class="about">
        <h2>About Our University</h2>
        <p>We are a leading university with a global reputation for excellence. Our campus is located in the heart of a vibrant city, offering a wide range of academic programs and extracurricular activities.</p>
    </div>

    <!-- Programs Section -->
    <div id="programs" class="programs">
        <h2>Our Programs</h2>
        <div class="programs-list">
            <div class="program">
                <h3>Computer Science</h3>
                <p>Study the latest technologies and programming languages.</p>
                <a href="#">Learn More</a>
            </div>
            <div class="program">
                <h3>Business Administration</h3>
                <p>Become a leader in the business world.</p>
                <a href="#">Learn More</a>
            </div>
            <div class="program">
                <h3>Engineering</h3>
                <p>Build the future with cutting-edge technologies.</p>
                <a href="#">Learn More</a>
            </div>
        </div>
    </div>

    <!-- Contact Section -->
    <div id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Have any questions? Feel free to reach out to us!</p>
        <a href="mailto:info@university.com">Email Us</a>
    </div>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 My University | All Rights Reserved</p>
        <p><a href="#">Privacy Policy</a> | <a href="#">Terms of Service</a></p>
    </footer>
</body>
</html>
