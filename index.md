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
  <!-- Inline CSS to mimic jeremybejarano.com with a photo in the left column -->
  <style>
    /* Base reset and simple typography */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
      color: #333;
      line-height: 1.5;
      background-color: #fff;
      margin: 2rem;
    }
    a {
      color: #0073e6;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }

    /* Container for the two-column layout */
    .container {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap; /* Stacks columns on mobile */
    }

    /* LEFT COLUMN */
    .left-column {
      flex: 1 1 300px;
      max-width: 350px;
      margin-right: 3rem;
    }
    .profile-photo {
      display: block;
      margin-bottom: 1rem;
      width: 120px;
      height: auto;
      border-radius: 50%; /* Circular photo */
    }
    .name {
      font-size: 2rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }
    .location {
      margin-bottom: 1rem;
      color: #666;
    }
    .links {
      margin-top: 1rem;
    }
    .links a {
      display: block;
      margin-bottom: 0.5rem;
      font-weight: 500;
    }

    /* RIGHT COLUMN */
    .right-column {
      flex: 2 1 400px;
    }
    .section {
      margin-bottom: 2rem;
    }
    .section h2 {
      margin-bottom: 1rem;
      font-size: 1.25rem;
      border-bottom: 1px solid #eee;
      padding-bottom: 0.5rem;
      font-weight: 600;
    }
    .section ul {
      list-style: disc;
      margin-left: 1.5rem;
    }
    .section p, .section li {
      margin-bottom: 0.75rem;
    }

    /* RESPONSIVE: stack columns on narrow screens */
    @media (max-width: 800px) {
      .container {
        flex-direction: column;
      }
      .left-column {
        max-width: 100%;
        margin-right: 0;
        margin-bottom: 2rem;
      }
      .right-column {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>

<div class="container">
  <!-- LEFT COLUMN -->
  <div class="left-column">
    <!-- Profile Photo -->
    <img src="/assets/images/profile.jpg" alt="Profile Photo" class="profile-photo" />

    <div class="name">Aadi Deshpande</div>
    <div class="location">Chicago, IL</div>

    <p>
      I'm currently pursuing a Master of Science in Financial Mathematics at
      The University of Chicago (expected Dec 2025). I'm actively seeking
      Summer 2025 internships in quantitative finance, data science, 
      and algorithmic trading.
    </p>

    <div class="links">
      <a href="mailto:aadi@uchicago.edu">aadi@uchicago.edu</a>
      <a href="https://www.linkedin.com/in/aadi-deshpande-b13045166/">LinkedIn Profile</a>
      <!-- Optional GitHub link:
      <a href="https://github.com/username">GitHub</a>
      -->
    </div>
  </div>

  <!-- RIGHT COLUMN -->
  <div class="right-column">

    <!-- Education Section -->
    <div class="section">
      <h2>Education</h2>
      <ul>
        <li>
          <strong>M.S. Financial Mathematics</strong>, The University of Chicago<br/>
          <em>Expected Dec 2025</em>
        </li>
        <li>
          <strong>B.Tech. in Computer Science</strong>, Manipal Institute of Technology<br/>
          <em>July 2018 – July 2022</em>
        </li>
      </ul>
    </div>

    <!-- Experience Section -->
    <div class="section">
      <h2>Experience</h2>
      <ul>
        <li>
          <strong>Quantitative Researcher</strong> - Univ. of Chicago Project Lab<br/>
          <em>Jan 2025 – Present</em><br/>
          Developed latent factor models using PCA to enhance factor investing strategies in corporate bonds.
        </li>
        <li>
          <strong>Engineering Analyst</strong> - Goldman Sachs<br/>
          <em>Aug 2022 – July 2024</em><br/>
          Built distributed microservices with Apache Kafka, improved SQL issue resolution times, 
          and developed NLP solutions for invoice processing.
        </li>
      </ul>
    </div>

    <!-- Skills Section -->
    <div class="section">
      <h2>Skills</h2>
      <ul>
        <li>Languages: Python, C++, Java, SQL</li>
        <li>Frameworks: Docker, FastAPI, Spring Boot, Django REST</li>
        <li>Quant Methods: Portfolio Optimization, Risk Management, Machine Learning</li>
      </ul>
    </div>

    <!-- Projects Section -->
    <div class="section">
      <h2>Projects</h2>
      <ul>
        <li>
          <strong>Portfolio Optimization</strong><br/>
          Mean-Variance model incorporating TIPS to mitigate inflation risk.
        </li>
        <li>
          <strong>Predictive Modeling for Loan Repayment</strong><br/>
          Achieved 89% accuracy on 400k+ loan records using Keras/TensorFlow.
        </li>
        <li>
          <strong>Scalable Data Platform</strong><br/>
          Python FastAPI backend, Docker-based deployment, and a robust Data Lake architecture.
        </li>
      </ul>
    </div>

  </div>
</div>

</body>
</html>
