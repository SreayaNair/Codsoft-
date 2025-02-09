<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio</title>
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
            background: url('https://cdn.pixabay.com/photo/2016/12/06/03/54/woman-1887997_960_720.jpg') no-repeat center center/cover;
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

        .about img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            margin-top: 20px;
        }

        /* Skills Section */
        .skills {
            padding: 60px 20px;
            text-align: center;
            background-color: #fff;
        }

        .skills h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .skills ul {
            list-style-type: none;
            padding: 0;
        }

        .skills ul li {
            font-size: 1.2rem;
            margin: 10px 0;
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

    </style>
</head>
<body>

    <!-- Navbar -->
    <nav>
        <div class="logo">My Portfolio</div>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <div class="hero">
        <div>
            <h1>Welcome to My Portfolio</h1>
            <p>I'm a passionate web developer!</p>
            <a href="#contact" class="cta-button">Contact Me</a>
        </div>
    </div>

    <!-- About Section -->
    <div id="about" class="about">
        <h2>About Me</h2>
        <p>I am a web developer with a strong passion for creating beautiful and functional websites. I specialize in front-end development, and I'm always looking to learn and improve my skills.</p>
        <img src="https://cdn.pixabay.com/photo/2016/12/06/03/54/woman-1887997_960_720.jpg" alt="pict">
    </div>

    <!-- Skills Section -->
    <div id="skills" class="skills">
        <h2>Skills</h2>
        <ul>
            <li>HTML & CSS</li>
            <li>JavaScript</li>
            <li>Responsive Web Design</li>
        </ul>
    </div>

    <!-- Contact Section -->
    <div id="contact" class="contact">
        <h2>Contact Me</h2>
        <p>Have any questions? Feel free to reach out to me!</p>
        <a href="mailto:info@portfolio.com">Email Me</a>
    </div>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 My Portfolio | All Rights Reserved</p>
        <p><a href="#">Privacy Policy</a> | <a href="#">Terms of Service</a></p>
    </footer>

</body>
</html>
