---
layout: null
title: "Home"
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ page.title }}</title>
  <meta name="description" content="Showcasing my work">
  
  <!-- Inline CSS -->
  <style>
    /* General Reset/Basic Styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #f8f9fa;
      color: #333;
      line-height: 1.6;
    }

    /* Header and Nav */
    header {
      background: #0077b6;
      color: #fff;
      padding: 20px;
    }
    header h1 {
      margin: 0;
      font-size: 1.8rem;
    }
    nav ul {
      list-style: none;
      margin: 10px 0 0 0;
      padding: 0;
      display: flex;
      gap: 15px;
    }
    nav ul li {
      display: inline-block;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }

    /* Main Content */
    main {
      display: flex;
      flex-wrap: wrap; /* so content wraps on smaller screens */
      padding: 20px;
      align-items: center;
    }

    .profile-photo {
      width: 180px;       /* Adjust as desired */
      height: auto;
      border-radius: 10px;
      margin-right: 30px; /* Space between photo and text */
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    }

    .text-section {
      flex: 1;
      min-width: 300px;   /* Ensures text doesn't get too narrow */
    }

    /* Footer */
    footer {
      text-align: center;
      background: #023e8a;
      color: #fff;
      padding: 10px 20px;
    }
  </style>
</head>
<body>

  <!-- Header with Basic Nav -->
  <header>
    <h1>My Portfolio</h1>
    <nav>
      <ul>
        <li><a href="{{ '/' | relative_url }}">Home</a></li>
        <li><a href="{{ '/about' | relative_url }}">About</a></li>
        <li><a href="{{ '/projects' | relative_url }}">Projects</a></li>
      </ul>
    </nav>
  </header>

  <!-- Main Content: Photo on Left, Text on Right -->
  <main>
    <img src="/assets/images/profile.jpg" alt="Profile Photo" class="profile-photo">

    <div class="text-section">
      <h2>Hello, I'm Aadi Deshpande</h2>
      <p>
        I’m currently pursuing a <strong>Master of Science in Financial Mathematics</strong> at
        the University of Chicago (expected December 2025), with a B.Tech. in Computer Science from
        Manipal Institute of Technology.
      </p>
      <p>
        I’ve held roles at Goldman Sachs and the University of Chicago Project Lab, focusing on
        quantitative research, distributed microservices, and data analytics. I’m <strong>actively 
        seeking Summer 2025 internship</strong> opportunities in quantitative finance, data science, 
        and related fields.
      </p>

      <h3>Skills & Interests</h3>
      <ul>
        <li>Python, C++, Java, SQL</li>
        <li>Portfolio Optimization, Risk Management</li>
        <li>Machine Learning (TensorFlow, Keras)</li>
      </ul>

      <h3>Contact</h3>
      <ul>
        <li>Email: <a href="mailto:aadi@uchicago.edu">aadi@uchicago.edu</a></li>
        <li>LinkedIn: 
          <a href="https://www.linkedin.com/in/aadi-deshpande-b13045166/" target="_blank">
            linkedin.com/in/aadi-deshpande-b13045166/
          </a>
        </li>
        <li>Location: Chicago, IL</li>
      </ul>
    </div>
  </main>

  <!-- Footer -->
  <footer>
    <p>&copy; {{ site.time | date: "%Y" }} My Portfolio. All rights reserved.</p>
  </footer>

</body>
</html>
