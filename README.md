# 🌐 Developer Portfolio (HTML + CSS)

This is a **one-page developer portfolio** with a **rotating background animation** (HTML + CSS only).  
You can use this code in **GitHub Pages, Netlify, or local browser**.

---

## 🚀 Features
- Rotating tech icons (React, JS, HTML, CSS)
- Clean dark UI
- Fully responsive
- Single HTML file

---

## 📌 How to Use
1. Create a file named `index.html`
2. Copy the code below
3. Paste it into `index.html`
4. Open in browser or deploy 🚀

---

## 💻 Full Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sakshi | Developer Portfolio</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #0f172a;
      color: white;
    }

    .hero {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      overflow: hidden;
    }

    .rotate-box {
      position: absolute;
      width: 420px;
      height: 420px;
      animation: spin 25s linear infinite;
      opacity: 0.35;
    }

    .icon {
      position: absolute;
      width: 60px;
    }

    .icon1 { top: 0; left: 50%; transform: translateX(-50%); }
    .icon2 { bottom: 0; left: 10%; }
    .icon3 { right: 0; top: 45%; }
    .icon4 { left: 0; top: 45%; }

    @keyframes spin {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

    .content {
      position: relative;
      z-index: 10;
      text-align: center;
    }

    .content h1 {
      font-size: 48px;
    }

    .content span {
      color: #22d3ee;
    }

    .content p {
      margin-top: 10px;
      font-size: 20px;
      color: #cbd5f5;
    }

    .btns {
      margin-top: 25px;
    }

    .btns a {
      text-decoration: none;
      padding: 12px 25px;
      margin: 5px;
      border-radius: 8px;
      color: white;
      border: 1px solid #22d3ee;
    }

    .btn-primary {
      background: #22d3ee;
      color: black;
    }

    section {
      padding: 80px 20px;
      text-align: center;
    }

    section h2 {
      font-size: 36px;
      margin-bottom: 20px;
    }

    .about,
    .projects {
      background: #020617;
    }

    .skills span {
      display: inline-block;
      margin: 10px;
      padding: 12px 20px;
      background: #1e293b;
      border-radius: 20px;
    }

    .project-box {
      max-width: 900px;
      margin: auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: #1e293b;
      padding: 25px;
      border-radius: 12px;
    }

    footer {
      padding: 30px;
      background: black;
      text-align: center;
      color: gray;
    }
  </style>
</head>

<body>

  <div class="hero">
    <div class="rotate-box">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" class="icon icon1">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" class="icon icon2">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" class="icon icon3">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" class="icon icon4">
    </div>

    <div class="content">
      <h1>Hi, I'm <span>Sakshi</span></h1>
      <p>Frontend Developer | HTML • CSS • JavaScript</p>

      <div class="btns">
        <a href="#projects" class="btn-primary">Projects</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </div>

  <section class="about">
    <h2>About Me</h2>
    <p>I am a passionate frontend developer who loves UI & animations.</p>
  </section>

  <section class="skills">
    <h2>Skills</h2>
    <span>HTML</span>
    <span>CSS</span>
    <span>JavaScript</span>
    <span>GitHub</span>
  </section>

  <section id="projects" class="projects">
    <h2>Projects</h2>
    <div class="project-box">
      <div class="card">Portfolio Website</div>
      <div class="card">Calculator App</div>
      <div class="card">Login Form</div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Email:muskansoni.code@gmail.com</p>
  </section>

  <footer>
    © 2026 Muskan Soni | Portfolio
  </footer>

</body>
</html>
