# PRODIGY_TrackCode_TaskNumber4
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      scroll-behavior: smooth;
    }

    /* Navbar */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: #333;
      color: #fff;
      display: flex;
      justify-content: space-between;
      padding: 15px 30px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.2);
      z-index: 1000;
    }

    nav a {
      color: #fff;
      margin-left: 20px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      color: #f39c12;
    }

    /* Hero Section */
    .hero {
      height: 100vh;
      background: linear-gradient(135deg, #74ABE2, #5563DE);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: #fff;
      text-align: center;
      padding: 20px;
    }

    .hero h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 20px;
    }

    .hero button {
      padding: 10px 20px;
      background: #fff;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      transition: transform 0.2s ease;
    }

    .hero button:hover {
      transform: scale(1.05);
      background: #f0f0f0;
    }

    /* About Section */
    .section {
      padding: 80px 20px;
      text-align: center;
    }

    .section h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      color: #333;
    }

    .section p {
      max-width: 700px;
      margin: 0 auto;
      font-size: 1rem;
      color: #555;
    }

    /* Projects Section */
    .projects {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 40px;
    }

    .project-card {
      background: #f7f7f7;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      padding: 20px;
      width: 280px;
      transition: transform 0.2s ease;
    }

    .project-card:hover {
      transform: translateY(-5px);
    }

    .project-card h3 {
      margin-bottom: 10px;
    }

    /* Contact Section */
    .contact {
      background: #333;
      color: #fff;
      padding: 40px 20px;
    }

    .contact h2 {
      margin-bottom: 20px;
    }

    .contact p {
      margin: 5px 0;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 15px;
      background: #222;
      color: #fff;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <!-- Navbar -->
  <nav>
    <div>My Portfolio</div>
    <div>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Hi, I'm Mantavya Singh</h1>
    <p>Web Developer | Designer | Tech Enthusiast</p>
    <button onclick="document.getElementById('projects').scrollIntoView()">View My Work</button>
  </section>

  <!-- About Section -->
  <section class="section" id="about">
    <h2>About Me</h2>
    <p>
      I'm a passionate web developer skilled in creating modern, responsive websites and web applications.
      I enjoy solving real-world problems and learning new technologies to improve my craft.
    </p>
  </section>

  <!-- Projects Section -->
  <section class="section" id="projects">
    <h2>My Projects</h2>
    <div class="projects">
      <div class="project-card">
        <h3>Portfolio Website</h3>
        <p>A modern personal portfolio showcasing my skills and projects.</p>
      </div>
      <div class="project-card">
        <h3>Weather App</h3>
        <p>Fetches real-time weather data using OpenWeather API.</p>
      </div>
      <div class="project-card">
        <h3>Stopwatch App</h3>
        <p>A responsive stopwatch with lap recording feature.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section class="contact" id="contact">
    <h2>Contact Me</h2>
    <p>Email: yourname@example.com</p>
    <p>Phone: +91 9876543210</p>
    <p>LinkedIn: linkedin.com/in/yourprofile</p>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Mantavya Singh | All Rights Reserved
  </footer>
</body>
</html>
