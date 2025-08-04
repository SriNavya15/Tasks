# Tasks
A responsive and visually appealing landing page built using HTML and CSS.
Landing Page
A clean and responsive landing page created using **HTML5 and CSS3**, with Flexbox layout and animations.

Features
- Responsive design
- Animated hero section
- Stylish header and footer
- Flexbox and media queries
- Simple and lightweight code

 Screenshot<img width="1904" height="791" alt="image" src="https://github.com/user-attachments/assets/b7f9d876-291e-43f6-b106-699f07bf2178" />

Tech Used
- HTML5
- CSS3 (Flexbox, media queries)
- Google Fonts


Folder Structure
├── index.html
├── style.css
└── screenshots/
└── preview.png






Index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Awesome Landing Page</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600&display=swap" rel="stylesheet">
</head>
<body>


  <!-- Header -->
  <header class="header">
    <div class="container">
      <div class="logo">✨ Logarogya</div>
      <nav class="navbar">
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#">About Us</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>


  <!-- Hero -->
  <section class="hero">
    <div class="hero-content">
      <h1>Redefining Patient Experience</h1>
      <p>One platform to connect, manage, and simplify healthcare in government hospitals.</p>
      <a href="#" class="btn">Join the Mission</a>
    </div>
  </section>


  <!-- Footer -->
  <footer class="footer">
    <div class="container">
      <p>&copy; 2025 Logarogya. Crafted with ❤️</p>
      <div class="social">
        <a href="#">🌐</a>
        <a href="#">🐦</a>
        <a href="#">📸</a>
      </div>
    </div>
  </footer>


</body>
</html>




style.css
/* Font and Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


body {
  font-family: 'Outfit', sans-serif;
  background: linear-gradient(135deg, #dfe9f3 0%, #ffffff 100%);
  color: #333;
}


.container {
  width: 90%;
  max-width: 1200px;
  margin: auto;
}


/* Header */
.header {
  background: rgba(255, 255, 255, 0.95);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
  position: sticky;
  top: 0;
  z-index: 1000;
  padding: 20px 0;
}


.logo {
  font-size: 28px;
  font-weight: 600;
  color: #0077ff;
}


.navbar {
  display: flex;
  justify-content: flex-end;
}


.nav-links {
  list-style: none;
  display: flex;
  gap: 30px;
}


.nav-links a {
  text-decoration: none;
  color: #333;
  font-weight: 500;
  transition: all 0.3s;
}


.nav-links a:hover {
  color: #0077ff;
  transform: scale(1.05);
}


/* Hero */
.hero {
  background: linear-gradient(135deg, #0077ff, #00d2ff);
  color: white;
  padding: 120px 20px;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  animation: fadeIn 1s ease-in-out;
}


.hero h1 {
  font-size: 50px;
  font-weight: 600;
  margin-bottom: 20px;
  animation: slideDown 1s ease-in-out;
}


.hero p {
  font-size: 20px;
  margin-bottom: 30px;
  max-width: 600px;
  line-height: 1.5;
}


.btn {
  background-color: #fff;
  color: #0077ff;
  padding: 14px 32px;
  border-radius: 30px;
  font-weight: bold;
  text-decoration: none;
  box-shadow: 0 4px 15px rgba(0, 119, 255, 0.3);
  transition: all 0.3s;
}


.btn:hover {
  background-color: #f0f0f0;
  transform: translateY(-2px);
}


/* Footer */
.footer {
  background-color: #1a1a1a;
  color: #bbb;
  padding: 30px 0;
  text-align: center;
}


.footer .social a {
  margin: 0 10px;
  text-decoration: none;
  font-size: 20px;
  color: #bbb;
  transition: color 0.3s;
}


.footer .social a:hover {
  color: #fff;
}


/* Animations */
@keyframes fadeIn {
  from { opacity: 0; transform: scale(0.98); }
  to { opacity: 1; transform: scale(1); }
}


@keyframes slideDown {
  from { opacity: 0; transform: translateY(-30px); }
  to { opacity: 1; transform: translateY(0); }
}


/* Responsive */
@media (max-width: 768px) {
  .nav-links {
    flex-direction: column;
    gap: 10px;
    text-align: right;
  }


  .hero h1 {
    font-size: 36px;
  }


  .hero p {
    font-size: 16px;
  }


  .btn {
    padding: 12px 25px;
  }
}
