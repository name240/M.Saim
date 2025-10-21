<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>M.S.M Firecore V2</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html, body {
      height: 100%;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      background: radial-gradient(circle at top, #1a0000, #000000 80%);
      font-family: 'Segoe UI', sans-serif;
    }

    .logo-box {
      position: relative;
      width: 360px;
      height: 200px;
      background: rgba(255, 255, 255, 0.05);
      border-radius: 20px;
      backdrop-filter: blur(16px);
      box-shadow:
        0 0 30px rgba(255, 0, 0, 0.25),
        0 0 70px rgba(255, 0, 0, 0.3),
        inset 0 0 10px rgba(255, 255, 255, 0.06);
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.3s ease-in-out;
      cursor: pointer;
    }

    .logo-box:hover {
      box-shadow:
        0 0 40px rgba(255, 0, 0, 0.4),
        0 0 90px rgba(255, 50, 0, 0.5),
        inset 0 0 12px rgba(255, 255, 255, 0.08);
    }

    .logo-text {
      font-size: 44px;
      font-weight: bold;
      letter-spacing: 12px;
      background: linear-gradient(to right, #ff4d4d, #ff0000, #ff4d00);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-shadow:
        0 0 10px rgba(255, 0, 0, 0.7),
        0 0 20px rgba(255, 50, 0, 0.6),
        0 0 30px rgba(255, 80, 0, 0.5);
      z-index: 2;
      animation: glow 3.5s ease-in-out infinite;
    }

    .light-wave {
      position: absolute;
      top: 0;
      left: -100%;
      width: 200%;
      height: 100%;
      background: linear-gradient(
        120deg,
        transparent 0%,
        rgba(255, 255, 255, 0.07) 50%,
        transparent 100%
      );
      transform: skewX(-20deg);
      animation: waveMove 5s linear infinite;
      z-index: 1;
    }

    .reflection-top {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 50%;
      background: linear-gradient(to bottom, rgba(255,255,255,0.07), transparent);
      border-top-left-radius: 20px;
      border-top-right-radius: 20px;
      z-index: 1;
      pointer-events: none;
    }

    @keyframes glow {
      0%, 100% {
        text-shadow:
          0 0 10px rgba(255, 0, 0, 0.7),
          0 0 20px rgba(255, 50, 0, 0.6),
          0 0 30px rgba(255, 80, 0, 0.5);
      }
      50% {
        text-shadow:
          0 0 15px rgba(255, 50, 0, 0.9),
          0 0 25px rgba(255, 100, 0, 0.7),
          0 0 40px rgba(255, 120, 0, 0.6);
      }
    }

    @keyframes waveMove {
      0% {
        left: -100%;
      }
      100% {
        left: 100%;
      }
    }

    /* Mobile Responsive */
    @media (max-width: 400px) {
      .logo-box {
        width: 90%;
        height: 180px;
      }

      .logo-text {
        font-size: 34px;
        letter-spacing: 8px;
      }
    }
  </style>
</head>
<body>

<center>  <div class="logo-box" onclick="restartWave()">
    <div class="light-wave"></div>
    <div class="reflection-top"></div>
    <div class="logo-text">M.S.M</div>
  </div></center>

  <script>
    function restartWave() {
      const wave = document.querySelector('.light-wave');
      wave.style.animation = 'none';
      void wave.offsetWidth;
      wave.style.animation = 'waveMove 5s linear infinite';
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
