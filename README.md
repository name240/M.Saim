<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>M.S.M Logo - Centered Version</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html, body {
      width: 100%;
      height: 100%;
      background: linear-gradient(to bottom right, #0f2027, #203a43, #2c5364);
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .logo-panel {
      width: 320px;
      height: 200px;
      background: rgba(255, 255, 255, 0.05);
      border-radius: 20px;
      box-shadow:
        0 0 20px rgba(0, 255, 255, 0.1),
        0 0 40px rgba(0, 255, 255, 0.15),
        inset 0 0 20px rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(10px);
      position: relative;
      overflow: hidden;
      padding: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .logo-panel:hover {
      transform: scale(1.03);
    }

    .logo-text {
      color: #ffffff;
      font-size: 40px;
      font-weight: bold;
      letter-spacing: 10px;
      z-index: 2;
      text-shadow:
        0 0 5px #00f2fe,
        0 0 10px #4facfe,
        0 0 15px #00f2fe;
      animation: glowPulse 3s ease-in-out infinite;
    }

    .shine-overlay {
      position: absolute;
      top: -50%;
      left: -100%;
      width: 200%;
      height: 200%;
      background: linear-gradient(120deg, rgba(255,255,255,0.05), rgba(255,255,255,0.3), rgba(255,255,255,0.05));
      transform: rotate(20deg);
      animation: shineSlide 6s linear infinite;
      pointer-events: none;
    }

    .lines {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: 1;
      background: repeating-linear-gradient(
        to bottom,
        rgba(255, 255, 255, 0.02),
        rgba(255, 255, 255, 0.02) 2px,
        transparent 2px,
        transparent 8px
      );
    }

    @keyframes shineSlide {
      0% { transform: translateX(-100%) rotate(20deg); }
      100% { transform: translateX(100%) rotate(20deg); }
    }

    @keyframes glowPulse {
      0%, 100% {
        text-shadow:
          0 0 5px #00f2fe,
          0 0 10px #4facfe,
          0 0 15px #00f2fe;
      }
      50% {
        text-shadow:
          0 0 10px #00f2fe,
          0 0 20px #4facfe,
          0 0 30px #00f2fe;
      }
    }

    /* Responsive */
    @media screen and (max-width: 400px) {
      .logo-panel {
        width: 90%;
        height: 180px;
      }

      .logo-text {
        font-size: 32px;
        letter-spacing: 6px;
      }
    }
  </style>
</head>
<body>

  <div class="logo-panel" onclick="restartShine()">
    <div class="lines"></div>
    <div class="shine-overlay"></div>
    <div class="logo-text">M.S.M</div>
  </div>

  <script>
    function restartShine() {
      const shine = document.querySelector('.shine-overlay');
      shine.style.animation = 'none';
      void shine.offsetWidth;
      shine.style.animation = 'shineSlide 6s linear infinite';
    }
  </script>

</body>
</html>




<html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,text-align:device,initial-scale=device"/>
	<style>

h1{font-size:5vw;}
p{font-size:3vw;}
	</style>
  <title>The Radiance School System</title>
  <style>
    /* Basic Reset */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      scroll-behavior: smooth;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background: linear-gradient(to right, #fefcea, #f1da36);
      min-height: 100vh;
      color: #333;
	
	  
    }

    header {
      background: #002c6b;
      color: #fff;
      padding: 20px;
      text-align: center;
      box-shadow: 0 4px 6px rgba(0,0,0,0.2);
    }

    nav {
	width:100%
	min-height:100vh;
      display: flex;
      justify-content: center;
	  flex-direction:column;
      background: #0056b3;
      padding: 10px;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    .container {
      text-align: center;
      padding: 40px 20px;
    }

    .container img {
      width: 300px;
      max-width: 90%;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }

    .school-name {
      margin-top: 20px;
      font-size: 32px;
      font-weight: bold;
      color: #002c6b;
      text-shadow: 1px 1px 2px #999;
    }

    .tagline {
      font-size: 18px;
      color: #666;
      margin-top: 10px;
    }

    section {
      padding: 60px 20px;
    }

    section h2 {
      color: #002c6b;
      margin-bottom: 20px;
    }
section h1 {
      color: #002c6b;
      margin-bottom: 20px;
    }
    footer {
      background: #002c6b;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to The Radiance School System</h1>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <div id="home" class="container">
    <img src="C:\Users\HP\Desktop\New folder\School Logo.jpg;" alt="School Logo" />

    <div class="school-name">THE RADIANCE SCHOOL SYSTEM</div>
    <div class="tagline">Glow the minds with knowledge</div>
  </div>

  <section id="about">
	<h2>About </h2>
    <p>
      The Radiance School System is dedicated to empowering students through knowledge
      creativity, and moral values. We provide a nurturing environment that encourages
      learning and personal growth for every student.
    </p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p>Email: info@theradianceschool.edu.pk</p>
    <p>Phone: +92-300-0000000</p>
  </section>
  <section id="created By:">
  <h1>Created By:</h1>
  <p>M.Saim Majoka</p>
  </section>
  <footer>
    &copy; 2025 The Radiance School System.
  </footer>

  <script>
    // Smooth scroll for nav links
    document.querySelectorAll('nav a').forEach(link => {
      link.addEventListener('click', e => {
        e.preventDefault();
        const target = document.querySelector(link.getAttribute('href'));
        if (target) {
          target.scrollIntoView({ behavior: 'smooth' });
        }
      });
    });
  </script>

</body>
</html>
