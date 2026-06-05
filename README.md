<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Jawad Marmar Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root{
  --bg:#0b1220;
  --surface:#111a2e;
  --ink:#eaf0ff;
  --muted:#a7b3c7;
  --line:#24324d;
  --blue:#3b82f6;
  --darkblue:#1e3a8a;
  --amber:#f59e0b;
}

*{margin:0;padding:0;box-sizing:border-box;font-family:Inter,sans-serif;}

body{
  background:var(--bg);
  color:var(--ink);
  overflow-x:hidden;
}

header{
  position:sticky;top:0;
  background:rgba(11,18,32,0.8);
  backdrop-filter:blur(10px);
  border-bottom:1px solid var(--line);
  padding:15px 20px;
  display:flex;
  justify-content:space-between;
}

nav a{
  margin:0 10px;
  color:var(--muted);
  text-decoration:none;
}
nav a:hover{color:var(--blue);}

.hero{
  padding:80px 20px;
  text-align:center;
}

.hero h1{
  font-size:34px;
  margin:15px 0;
}

.btn{
  padding:10px 15px;
  border:1px solid var(--line);
  border-radius:6px;
  margin:5px;
  text-decoration:none;
  color:var(--ink);
}

.btn.primary{
  background:var(--blue);
  border:none;
}

.section{
  padding:60px 20px;
  max-width:900px;
  margin:auto;
}

.card{
  background:var(--surface);
  padding:20px;
  border-radius:10px;
  margin:10px 0;
  border:1px solid var(--line);
  transition:0.3s;
}

.card:hover{
  transform:translateY(-5px);
}

footer{
  text-align:center;
  padding:20px;
  border-top:1px solid var(--line);
  color:var(--muted);
}

</style>
</head>

<body>

<header>
  <div><b>Jawad<span style="color:#f59e0b">Dev</span></b></div>
  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <h4 style="color:#f59e0b;">Web Developer</h4>
  <h1>Building clean, responsive web solutions.</h1>
  <p>Computer Science Student focused on Web Development & Backend Systems</p>

  <div>
    <a class="btn primary" href="#projects">View Projects</a>
    <a class="btn" href="#contact">Contact Me</a>
  </div>
</section>

<section id="about" class="section">
  <h2>About Me</h2>
  <div class="card">
    Passionate Computer Science student building real-world web applications.
  </div>
</section>

<section id="skills" class="section">
  <h2>Skills</h2>
  <div class="card">
    HTML • CSS • JavaScript • PHP • MySQL
  </div>
</section>

<section id="projects" class="section">
  <h2>Projects</h2>

  <div class="card">
    <h3>🦷 BrightSmile Dentistry</h3>
    <p>Full-stack booking system using PHP & MySQL.</p>
    <a href="https://github.com/jawaddmarmar/Brightsmile_project">GitHub Link</a>
  </div>

  <div class="card">
    <h3>Portfolio Website</h3>
    <p>Responsive developer portfolio built with HTML/CSS/JS.</p>
  </div>
</section>

<section id="contact" class="section">
  <h2>Contact</h2>
  <div class="card">
    Email: jawaddmarmar@gmail.com <br>
    GitHub: github.com/jawaddmarmar
  </div>
</section>

<footer>
  © <span id="year"></span> Jawad Marmar
</footer>

<script>
document.getElementById("year").textContent = new Date().getFullYear();
</script>

</body>
</html>
