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
