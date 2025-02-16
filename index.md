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
  <!-- Inline CSS for a minimal 2-column design -->
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

    /* Container to center the two-column layout */
    .container {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap; /* so columns can stack on mobile */
    }

    /* LEFT COLUMN */
    .left-column {
      flex: 1 1 300px;  /* Grow/shrink, min width 300px */
      max-width: 350px; /* Control how wide the left side can get */
      margin-right: 3rem;
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
      flex: 2 1 400px; /* Grows more than left column, min width 400px */
    }
    .section {
      margin-bottom: 2rem; /* Space between sections */
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
      <!-- Add GitHub link if desired:
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
          <strong>M.S. Financial Mathematics</strong>, The University of Chicago  
          <em>Expected Dec 2025</em>
        </li>
        <li>
          <strong>B.Tech. in Computer Science</strong>, Manipal Institute of Technology  
          <em>July 2018 - July 2022</em>
        </li>
      </ul>
    </div>

    <!-- Experience Section -->
    <div class="section">
      <h2>Experience</h2>
      <ul>
        <li>
          <strong>Quantitative Researcher</strong> - University of Chicago Project Lab  
          <em>Jan 2025 - Present</em>  
          Developed latent factor models using PCA to enhance factor investing strategies in corporate bonds.
        </li>
        <li>
          <strong>Engineering Analyst</strong> - Goldman Sachs  
          <em>Aug 2022 - July 2024</em>  
          Built distributed microservices with Apache Kafka, improved SQL issue resolution times, and implemented NLP techniques to streamline invoice processing.
        </li>
      </ul>
    </div>

    <!-- Skills Section -->
    <div class="section">
      <h2>Skills</h2>
      <ul>
        <li>Languages: Python, C++, Java, SQL</li>
        <li>Frameworks: Docker, FastAPI, Spring Boot, Django REST</li>
        <li>Quant Methods: Portfolio Optimization, Risk Management, Factor Investing</li>
      </ul>
    </div>

    <!-- Projects Section -->
    <div class="section">
      <h2>Projects</h2>
      <ul>
        <li>
          <strong>Portfolio Optimization</strong>  
          Implemented a Mean-Variance model incorporating inflation-indexed bonds (TIPS) for better risk mitigation.
        </li>
        <li>
          <strong>Predictive Modeling for Loan Repayment</strong>  
          Achieved 89% accuracy using neural networks (Keras/TensorFlow) on a dataset of 400k+ loan records.
        </li>
        <li>
          <strong>Scalable Data Platform</strong>  
          Developed a Python FastAPI backend with a Data Lake, advanced metadata catalog, and Docker-based deployment.
        </li>
      </ul>
    </div>

  </div>
</div>

</body>
</html>
