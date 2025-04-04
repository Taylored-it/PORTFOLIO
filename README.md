# PORTFOLIO
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css"/>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css"/>
</head>
<body>
  <!-- Navigation -->
  <nav>
    <input type="checkbox" class="checkbox" id="check" />
    <h1 class="nav_head">Karabo.</h1>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#contact">Contact</a></li>
      <a href="#contact"><button class="contact_btn">Contact Me</button></a>
    </ul>
    <label for="check" class="checkbtn">
      <i class="fas fa-bars"></i>
    </label>
  </nav>

  <!-- Home Section -->
  <section id="home" class="home">
    <img src="homepage.png" alt="Karabo smiling at camera" width="450px" height="400px" />
    <div class="description">
      <h1>Hello I'm<br><span>Karabo Selokela</span></h1>
      <h2>I'm a <span>Cybersecurity Engineer...</span></h2>
      <p>Welcome! Let's explore my website and get to know me and my work. I am so excited—yaaay!</p>
      <div class="font">
        <i class="fab fa-instagram"></i>
        <i class="fab fa-facebook"></i>
        <i class="fab fa-linkedin"></i>
        <i class="fas fa-phone"></i>
      </div>
      <a href="c:\Users\selok\Downloads\Graduate_Program[1].pdf" download><button>Download CV</button></a>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About Me</h2>
    <p>Hey there! I'm Karabo, a passionate cybersecurity engineer who loves solving digital mysteries, breaking systems (ethically 😎), and building safer online spaces.</p>
    <p>I’m currently diving deep into ethical hacking, penetration testing, and securing networks from threats. When I’m not doing that, I’m probably learning new tech, listening to deep house, or debugging life.</p>
  </section>

  <!-- Services Section -->
  <section id="services" class="services">
    <h2>My Services</h2>
    <div class="service-container">
      <div class="service-card">
        <i class="fas fa-shield-alt"></i>
        <h3>Cybersecurity Audits</h3>
        <p>Assess vulnerabilities and strengthen digital infrastructures with full audits and risk assessments.</p>
      </div>
      <div class="service-card">
        <i class="fas fa-lock"></i>
        <h3>Penetration Testing</h3>
        <p>Simulate attacks to expose weaknesses before the bad guys do. Ethical hacking at its finest.</p>
      </div>
      <div class="service-card">
        <i class="fas fa-code"></i>
        <h3>Web Security</h3>
        <p>Secure your web apps with code reviews, input sanitization, and protection against common attacks.</p>
      </div>
    </div>
  </section>

  <!-- Portfolio Section -->
  <section id="portfolio" class="portfolio">
    <h2>My Projects</h2>
    <div class="portfolio-container">
      <div class="project-card">
        <img src="phishing.png" alt="Project 1 Screenshot">
        <h3>Phishing Detection Tool</h3>
        <p>Built a smart tool to detect phishing links using machine learning. Because bad links belong in the trash 🗑️.</p>
      </div>
      <div class="project-card">
        <img src="aiscanner.png" alt="Project 2 Screenshot">
        <h3>Vulnerability Scanner</h3>
        <p>Automated script that scans web apps for OWASP Top 10 vulnerabilities. Made to catch bugs before they catch you.</p>
      </div>
      <div class="project-card">
        <img src="project3-image.jpg" alt="Project 3 Screenshot">
        <h3>Network Monitoring Dashboard</h3>
        <p>Created a sleek dashboard to monitor network traffic in real-time. Built with Python + Plotly Dash.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <p>Let's connect! Whether it's a collab, freelance work, or just tech talk — slide into my inbox below 👇</p>
    <form action="mailto:selokelakarabo98@gmail.com.com" method="post" enctype="text/plain">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>
</body>
</html>





* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
    scroll-behavior: smooth;
}
body {
    background-color: black;
    color: pink;
    text-align: center;
}

/* Navigation */
nav {
    background-color: black;
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    padding: 10px;
    font-size: larger;
}
.nav_head {
    font-size: 35px;
    color: white;
}
nav ul {
    display: flex;
    gap: 20px;
    list-style: none;
}
li a {
    color: white;
}
li a:hover {
    color: #ED2279;
}
.contact_btn {
    padding: 10px 30px;
    color: black;
    background-color: #ED2279;
    border-radius: 30px;
    font-size: larger;
    cursor: pointer;
    transition: .5s ease-in-out;
}
.contact_btn:hover {
    color: white;
    border: 2px solid #ED2279;
    background: transparent;
}
.checkbtn {
    font-size: 30px;
    cursor: pointer;
    display: none;
}
.checkbox {
    display: none;
}

/* Mobile responsiveness */
@media screen and (max-width: 952px) {
    .nav_head {
        font-size: 30px;
    }
    nav li a {
        font-size: 18px;
    }
}
@media screen and (max-width: 820px) {
    .checkbtn {
        display: block;
    }
    nav ul {
        flex-direction: column;
        background-color: black;
        position: fixed;
        top: 50px;
        right: -100%;
        width: 60%;
        height: 50vh;
        transition: right 0.5s;
    }
    .checkbox:checked ~ ul {
        right: 0;
    }
    nav li {
        text-align: center;
        width: 100%;
        padding: 10px 0;
    }
    .contact_btn {
        width: 90%;
        margin: 10px auto;
    }
}

/* Home section */
.home {
    padding: 220px 50px 100px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 3rem;
    color: white;
}
.description h1 {
    font-size: 30px;
    font-weight: 700;
}
.description h1 span {
    color: #ED2279;
    font-size: 55px;
}
.description h2 {
    margin-top: 20px;
    font-size: 30px;
    font-weight: 900;
}
.description h2 span {
    color: #ED2279;
}
.description p {
    width: 100%;
    max-width: 500px;
    margin: 20px auto;
}
.font i {
    margin: 25px 8px;
    border: 2px solid #ED2279;
    border-radius: 50%;
    padding: 13px;
    font-size: 20px;
    cursor: pointer;
    transition: 0.4s;
}
.font i:hover {
    background-color: #ED2279;
    transform: translateY(-15px);
    box-shadow: 0px 0px 15px #ED2279;
}
.description button {
    padding: 13px 20px;
    font-size: 20px;
    border-radius: 10px;
    background: linear-gradient(145deg, #ED2279, rgb(231, 201, 35));
    cursor: pointer;
    border: none;
}
.home img {
    background-color: #ED2279;
    padding: 10px;
    border-radius: 50%;
    box-shadow: 0px 0px 30px #ED2279;
    animation: float 2.5s ease-in-out infinite;
}
@keyframes float {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-15px);
    }
}

/* === About, Services, Portfolio, Contact === */

section {
    padding: 100px 20px;
    color: white;
    text-align: center;
}
.about,
.services,
.portfolio,
.contact {
    background-color: #1c1c1c;
    margin-top: 20px;
    border-radius: 15px;
    padding: 60px 30px;
}
.about p,
.services p,
.portfolio p,
.contact p {
    max-width: 700px;
    margin: 0 auto;
    line-height: 1.6;
}
.service-container,
.portfolio-container {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: center;
    margin-top: 30px;
}
.service-card,
.project-card {
    background-color: #2a2a2a;
    border-radius: 15px;
    padding: 30px;
    width: 300px;
    transition: 0.3s ease-in-out;
}
.service-card:hover,
.project-card:hover {
    transform: scale(1.05);
    box-shadow: 0 0 15px #ED2279;
}
.service-card i,
.project-card img {
    font-size: 40px;
    color: #ED2279;
    margin-bottom: 15px;
}
.project-card img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}
form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    max-width: 500px;
    margin: 30px auto 0;
}
form input,
form textarea {
    padding: 12px;
    border: none;
    border-radius: 8px;
    background-color: #333;
    color: white;
}
form button {
    padding: 12px;
    border: none;
    background-color: #ED2279;
    color: white;
    border-radius: 8px;
    cursor: pointer;
}
form button:hover {
    background-color: #c81c67;
}

