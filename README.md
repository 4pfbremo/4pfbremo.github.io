<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>
  <style>
    :root {
      --bg: #0f172a;
      --primary: #3b82f6;
      --text: #e2e8f0;
      --accent: #14b8a6;
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }
    body {
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }
    header {
      background: #1e293b;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    header h1 {
      font-size: 1.5rem;
      color: var(--primary);
    }
    nav a {
      margin: 0 1rem;
      color: var(--text);
      text-decoration: none;
      transition: color 0.3s;
    }
    nav a:hover {
      color: var(--accent);
    }

    .hero {
      padding: 4rem 2rem;
      text-align: center;
      animation: fadeIn 1.5s ease-in-out;
    }
    .hero h2 {
      font-size: 2.5rem;
      color: var(--primary);
      margin-bottom: 1rem;
    }
    .hero p {
      font-size: 1.2rem;
      color: #cbd5e1;
    }

    .projects, .about, .contact {
      padding: 3rem 2rem;
      max-width: 1000px;
      margin: auto;
    }
    .section-title {
      font-size: 2rem;
      margin-bottom: 1rem;
      color: var(--accent);
    }
    .project-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }
    .card {
      background: #1e293b;
      border-radius: 10px;
      padding: 1rem;
      transition: transform 0.3s ease;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 4px 20px rgba(0,0,0,0.4);
    }
    .card h3 {
      margin-bottom: 0.5rem;
      color: var(--primary);
    }

    form input, form textarea {
      width: 100%;
      padding: 0.8rem;
      margin: 0.5rem 0;
      border: none;
      border-radius: 5px;
    }
    form button {
      padding: 0.8rem 2rem;
      background: var(--primary);
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    footer {
      text-align: center;
      padding: 2rem;
      background: #1e293b;
      margin-top: 2rem;
      color: #94a3b8;
    }

    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(20px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @media (max-width: 600px) {
      .hero h2 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>🚀 My Portfolio</h1>
  <nav>
    <a href="#projects">Projects</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <h2>Hello, I'm Remixx</h2>
  <p>A passionate Web Developer crafting beautiful websites and experiences.</p>
</section>

<section class="projects" id="projects">
  <h2 class="section-title">🌟 Projects</h2>
  <div class="project-grid">
    <div class="card">
      <h3>Facebook Clone</h3>
      <p>A real-time social media app with Firebase backend.</p>
    </div>
    <div class="card">
      <h3>AutoPartsPro</h3>
      <p>E-commerce site for buying car parts, with payments & refunds.</p>
    </div>
    <div class="card">
      <h3>Music Hub</h3>
      <p>Stream your favorite tracks with this stylish music player.</p>
    </div>
  </div>
</section>

<section class="about" id="about">
  <h2 class="section-title">🙋 About Me</h2>
  <p>
    I'm a self-taught developer with a passion for building modern, responsive, and interactive web applications. I love turning ideas into reality with clean code and creative UI design.
  </p>
</section>

<section class="contact" id="contact">
  <h2 class="section-title">📬 Contact Me</h2>
  <form onsubmit="sendMessage(); return false;">
    <input type="text" placeholder="Your Name" required />
    <input type="email" placeholder="Your Email" required />
    <textarea rows="5" placeholder="Your Message" required></textarea>
    <button type="submit">Send Message</button>
  </form>
</section>

<footer>
  <p>© 2025 Remixx. All rights reserved.</p>
</footer>

<script>
  function sendMessage() {
    alert("📨 Message sent successfully!");
  }
</script>

</body>
</html># 4pfbremo.github.io
