# Final Project and Deployment

## Objectives
Build a fully functional web application.
Apply HTML, CSS, and JavaScript concepts learned.
Deploy the project using GitHub Pages, Netlify, or Vercel.

## Instructions
Choose one of the following project ideas:
Blog Website: Implement a multi-page site with navigation.
Ecommerce Website: Implement a multi-page site with navigation.

>[!NOTE]
> - Include at least:
> - A responsive design.
> - JavaScript interactivity.
> - A deployment link.

## Tasks

Create a well-structured HTML5 document.
Use at least 5 different HTML elements.
Ensure semantic correctness.

Good luck and happy coding! 🚀💻


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Responsive Website</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
    <style>
        /* Global Styles */
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }
        header {
            background-color: #2C3E50;  /* Dark blue background for header */
            color: white;
            padding: 1rem;
            text-align: center;
            background-image: url('https://via.placeholder.com/1600x400'); /* Header image */
            background-size: cover;
            background-position: center;
        }
        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }
        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            margin-bottom: 0;
        }
        nav ul li {
            margin: 0 1rem;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }
        nav ul li a:hover {
            color: #FF6347; /* Tomato color on hover */
        }
        main {
            padding: 2rem;
            text-align: center;
        }
        section {
            margin-bottom: 2rem;
        }
        footer {
            background-color: #2C3E50; /* Dark footer to match header */
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 3rem;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem;
        }
        /* Responsive Styles */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
            }
            nav ul li {
                margin: 0.5rem 0;
            }
        }
        /* Specific Page Styles */
        .home-section {
            background-color: #e9ecef;
            padding: 2rem;
            border-radius: 8px;
        }
        .about-section {
            background-color: #f8f9fa;
            padding: 2rem;
            border-radius: 8px;
        }
        .contact-form {
            max-width: 500px;
            margin: 0 auto;
            text-align: left;
        }
        .contact-form label {
            display: block;
            margin-top: 1rem;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 0.75rem;
            margin-top: 0.5rem;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .contact-form button {
            margin-top: 1rem;
            padding: 0.75rem 1.5rem;
            background-color: #FF6347; /* Tomato color for buttons */
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .contact-form button:hover {
            background-color: #FF4500; /* Darker tomato on hover */
        }
        .error-message {
            color: red;
            margin-top: 0.5rem;
        }
        .image-slider {
            display: flex;
            overflow: hidden;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
            position: relative;
            border-radius: 8px;
        }
        .slide {
            display: none;
            width: 100%;
            transition: opacity 0.5s ease;
        }
        .slide img {
            width: 100%;
            height: auto;
            border-radius: 8px;
        }
        .slide.active {
            display: block;
            opacity: 1;
        }
        .slider-nav {
            position: absolute;
            bottom: 1rem;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 0.5rem;
        }
        .slider-nav button {
            width: 1rem;
            height: 1rem;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.7);
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .slider-nav button:hover {
            background-color: rgba(255, 255, 255, 0.9);
        }
        .slider-nav button.active {
            background-color: #FF6347; /* Tomato color for active button */
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>My Website</h1>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="about.html">About</a></li>
                    <li><a href="contact.html">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <main>
        <div class="container">
            <section class="home-section">
                <h2>Welcome to the Home Page</h2>
                <p>This is the main page of our website.  It provides an overview of what we offer.  We hope you find it informative and easy to navigate.  Feel free to click the About and Contact links above.</p>
                <div class="image-slider">
                    <div class="slide active">
                        <img src="https://via.placeholder.com/600x400/FF6347/FFFFFF?text=Image+1" alt="Image 1">
                    </div>
                    <div class="slide">
                        <img src="https://via.placeholder.com/600x400/FF6347/FFFFFF?text=Image+2" alt="Image 2">
                    </div>
                    <div class="slide">
                        <img src="https://via.placeholder.com/600x400/FF6347/FFFFFF?text=Image+3" alt="Image 3">
                    </div>
                    <div class="slider-nav">
                        <button data-slide="0" class="active"></button>
                        <button data-slide="1"></button>
                        <button data-slide="2"></button>
                    </div>
                </div>
            </section>
        </div>
    </main>
    <footer>
        <div class="container">
            <p>&copy; 2025 My Website. All rights reserved.</p>
        </div>
    </footer>
    <script>
        const slider = document.querySelector('.image-slider');
        const slides = document.querySelectorAll('.slide');
        const navButtons = document.querySelectorAll('.slider-nav button');
        let currentSlide = 0;
        function showSlide(index) {
            slides.forEach(slide => slide.classList.remove('active'));
            navButtons.forEach(button => button.classList.remove('active'));
            slides[index].classList.add('active');
            navButtons[index].classList.add('active');
            currentSlide = index;
        }
        function nextSlide() {
            currentSlide = (currentSlide + 1) % slides.length;
            showSlide(currentSlide);
        }
        let slideInterval = setInterval(nextSlide, 3000);
        navButtons.forEach((button, index) => {
            button.addEventListener('click', () => {
                clearInterval(slideInterval);
                showSlide(index);
                slideInterval = setInterval(nextSlide, 3000);
            });
        });
        showSlide(currentSlide);
    </script>
</body>
</html>
