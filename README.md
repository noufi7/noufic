
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Portfolio</title>
  <style>
    /* === GLOBAL STYLE === */
    body {
      margin: 0;
      font-family: "Poppins", Arial, sans-serif;
      background: #111827;
      color: white;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(45deg, rgb(4, 159, 187), rgb(80, 246, 255));
      color: #1b233d;
      text-align: center;
      padding: 50px 20px;
      position: relative;
    }

    header img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 4px solid #1b233d;
      object-fit: fill;
      margin-bottom: 20px;
    }

    header h1 {
      font-size: 2.5rem;
      margin: 10px 0;
    }

    header p {
      font-size: 1.1rem;
      color: #1b233d;
    }

    nav {
      display: flex;
      justify-content: center;
      background: #1b233d;
      padding: 15px;
      gap: 20px;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav a:hover {
      color: rgb(80, 246, 255);
    }

    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }

    section h2 {
      text-align: center;
      color: rgb(80, 246, 255);
      margin-bottom: 30px;
      font-size: 2rem;
    }

    /* === ABOUT SECTION === */
    .about {
      display: flex;
      flex-wrap: wrap;
      gap: 30px;
      align-items: center;
      justify-content: center;
    }

    .about img {
      width: 300px;
      border-radius: 20px;
      object-fit: cover;
    }

    .about-text {
      max-width: 600px;
      font-size: 1.1rem;
      line-height: 1.6;
    }

    /* === PROJECTS SECTION === */
    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .project-card {
      background: #1b233d;
      border-radius: 15px;
      overflow: hidden;
      transition: transform 0.3s;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }

    .project-card:hover {
      transform: scale(1.05);
    }

    .project-card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }

    .project-card .info {
      padding: 15px;
    }

    .project-card .info h3 {
      margin: 0 0 10px;
      color: rgb(80, 246, 255);
    }

    /* === TRAVEL SECTION === */
    .travel-gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
    }

    .travel-gallery img {
      width: 100%;
      height: 200px;
      border-radius: 10px;
      object-fit: cover;
      transition: transform 0.3s;
    }

    .travel-gallery img:hover {
      transform: scale(1.05);
    }

    /* === CONTACT SECTION === */
    .contact {
      text-align: center;
    }

    .social-icons {
      margin-top: 20px;
      display: flex;
      justify-content: center;
      gap: 20px;
    }

    .social-icons a svg {
      width: 30px;
      fill: rgb(80, 246, 255);
      transition: fill 0.3s;
    }

    .social-icons a:hover svg {
      fill: white;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #0f172a;
      font-size: 0.9rem;
      color: rgba(255, 255, 255, 0.6);
    }

    @media (max-width: 700px) {
      header h1 {
        font-size: 2rem;
      }

      .about {
        flex-direction: column;
      }

      .about img {
        width: 80%;
      }
    }
  </style>
</head>
<body>
  <header>
    <img src="images/noufiprofilepic.png" alt="Your Photo" />
    <h1>Muhammed Noufal</h1>
    <p>IT Developer • Designer • Traveler</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#travel">Travel</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Me</h2>
    <div class="about">
      <img src="images/nofpic1.png" alt="About me picture">
      <div class="about-text">
        <p>
          Hi! I'm <b>Muhammed Noufal</b>, a passionate IT developer who loves building
          beautiful and functional websites. I enjoy creating modern designs, learning new technologies, and exploring the world through travel and photography.
        </p>
      </div>
    </div>
  </section>

  <section id="projects">
    <h2>My Projects</h2>
    <div class="projects">
      <div class="project-card">
        <img src="project1.jpg" alt="Project 1">
        <div class="info">
           <h3><a href="skills">Portfolio Website</a></h3>
          <p>A personal website showcasing my skills and projects.</p>
        </div>
      </div>

      <div class="project-card">
        <img src="project2.jpg" alt="Project 2">
        <div class="info">
          <h3>Travel Blog</h3>
          <p>Sharing my adventures, tips, and travel photography.</p>
        </div>
      </div>

      <div class="project-card">
        <img src="project3.jpg" alt="Project 3">
        <div class="info">
          <h3>Passion for Sports</h3>
          <p>Staying active through games that build focus, teamwork, and strategy.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="travel">
    <h2>Travel Gallery</h2>
    <div class="travel-gallery">
      <img src="travel1.jpg" alt="Travel photo 1">
      <img src="travel2.jpg" alt="Travel photo 2">
      <img src="travel3.jpg" alt="Travel photo 3">
      <img src="travel4.jpg" alt="Travel photo 4">
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <div class="contact">
      <p>Feel free to reach out via email or follow me on social media!</p>
      <div class="social-icons">
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30"><path d="M9.998 3C6.139 3 3 6.142 3 10.002v10c0 3.859 3.142 7 7.002 7h10c3.86 0 7-3.142 7-7.002v-10c0-3.86-3.142-7-7.002-7h-10zM22 7a1 1 0 110 2 1 1 0 010-2zm-7 2a6 6 0 100 12 6 6 0 000-12z"/></svg></a>
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M459.37 151.716c..."/></svg></a>
        <a href="#"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512"><path d="M524.531,69.836a1.5,1.5..."/></svg></a>
      </div>
    </div>
  </section>

  <footer>
    © 2025 Noufal. All rights reserved.
  </footer>
</body>
</html>
