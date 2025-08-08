# webtask2<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
  <title>Petchimuthu's Portfolio</title>

  <style>
    *{margin:0;padding:0;box-sizing:border-box}
    body{font-family:sans-serif;line-height:1.6;background:#f9f9f9;color:#333}
    header{background:#222;color:#fff;padding:1rem;text-align:center}
    .nav-links{list-style:none;display:flex;justify-content:center;gap:1rem;margin-top:1rem}
    .nav-links a{color:#fff;text-decoration:none;font-weight:bold}
    main{padding:2rem}
    h2{margin-top:2rem;color:#444}
    .card-container{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:1rem;margin-top:1rem}
    .card{background:#fff;padding:1rem;border-radius:8px;box-shadow:0 2px 5px rgba(0,0,0,0.1)}
    footer{text-align:center;padding:1rem;background:#111;color:#fff;margin-top:2rem}
    @media(max-width:600px){.nav-links{flex-direction:column;gap:0.5rem}}
    img{max-width:100%;border-radius:8px;margin-top:1rem}
  </style>
</head>
<body>
  <header>
    <h1>Raghu N Portfolio</h1>
    <p>ECE Student | Web Developer | Tech Enthusiast</p>
    <ul class="nav-links">
      <li><a href="#projects">Projects</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#about">About</a></li>
    </ul>
  </header>

  <main>
    <section id="projects">
      <h2>Highlighted Projects</h2>
      <div class="card-container" id="project-cards"></div>
    </section>

    <section id="skills">
      <h2>My Skills & Achievements</h2>
      <div class="card-container">
        <div class="card">
          <h3>Technical Skills</h3>
          <p>Java, python, HTML, CSS, JavaScript, SQL, React JS</p>
          <p>Learning: Excel with Power BI, SAP ABAP</p>
        </div>
        <div class="card">
          <h3>Certifications & Prizes</h3>
          <ul>
            <li>IEEE Filmography – 🥇 1st Prize</li>
            <li>IEEE Snapshot – 🥈 2nd Prize</li>
            <li>Circuit Design Project Expo – 🥈 2nd Prize (Magnetic Crane)</li>
            <li>Smart India Hackathon – Forest Fire Alerting System</li>
          </ul>
        </div>
        <div class="card">
          <h3>Workshops & Internships</h3>
          <ul>
            <li>Chip-Level Debugging Workshop</li>
            <li>PCB Designing (KiCAD)</li>
            <li>Internship – Tamil Nadu Railways</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="about">
      <h2>About Me</h2>
      <p>Hi! I’m sridevi.k, a 3rd-year Electronics and Communication Engineering student at Panimalar Engineering College. I'm passionate about tech, building creative projects, and always looking to grow.</p>
      <p><strong>Short-Term Goal:</strong> Get placed in a reputed company with a good package.</p>
      <p><strong>Long-Term Dream:</strong> Buy a <em>Jacob & Co.</em> watch 😎</p>
      <p><strong>Strengths:</strong> Quick learner, leadership, time management, team motivation</p>
      <p><strong>Weakness:</strong> I find it hard to say "no" to people.</p>
      <img loading="lazy" src="https://via.placeholder.com/500x300?text=My+Tech+Journey" alt="About Image">
    </section>
  </main>

  <footer>
    <p>© 2025 sridevi | Built with HTML, CSS & JS</p>
  </footer>

  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const projects = [
        {
          title: "AGRIVISION",
          description: "Smart agriculture platform with soil analysis, disease detection, govt schemes & disaster management."
        },
        {
          title: "Smart Parking System",
          description: "Conference-level project to detect and guide parking using sensors and automation."
        },
        {
          title: "Magnetic Crane Demo",
          description: "Electromagnetic crane showcased at EMF Expo – 2nd Prize Winner."
        },
        {
          title: "Fire Alert System",
          description: "IoT-based microcontroller project for detecting fire in restricted zones."
        }
      ];

      const container = document.getElementById("project-cards");

      projects.forEach(proj => {
        const card = document.createElement("div");
        card.className = "card";
       
        
        container.appendChild(card);
      });
    });
  </script>
</body>
</html>
