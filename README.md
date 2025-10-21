<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mesud Seid - Ethiopian Programmer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            text-align: center;
            padding: 40px 20px;
            color: white;
        }

        .logo-container {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            margin-bottom: 30px;
            display: inline-block;
        }

        .logo-image {
            max-width: 400px;
            height: auto;
            display: block;
            margin: 0 auto;
        }

        .logo-text {
            font-size: 2rem;
            font-weight: bold;
            color: #2c3e50;
            margin-top: 15px;
        }

        .tagline {
            font-size: 1.3rem;
            margin-bottom: 30px;
            opacity: 0.9;
            color: white;
        }

        .main-content {
            background: white;
            border-radius: 15px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            margin-top: 20px;
        }

        .profile-section {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 30px;
            margin-bottom: 40px;
        }

        @media (min-width: 768px) {
            .profile-section {
                flex-direction: row;
                text-align: left;
            }
        }

        .profile-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            font-weight: bold;
            border: 5px solid #FFD700;
        }

        .profile-info {
            flex: 1;
        }

        h1 {
            color: #2c3e50;
            margin-bottom: 15px;
            font-size: 2.5rem;
        }

        h2 {
            color: #667eea;
            margin: 30px 0 15px;
            border-bottom: 2px solid #f0f0f0;
            padding-bottom: 10px;
        }

        p {
            margin-bottom: 15px;
            font-size: 1.1rem;
        }

        .university {
            color: #764ba2;
            font-weight: bold;
            font-size: 1.2rem;
        }

        .goal {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            border-left: 5px solid #FFD700;
            margin: 20px 0;
        }

        .skills {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .skill-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
            border-top: 4px solid #667eea;
            transition: transform 0.3s ease;
        }

        .skill-card:hover {
            transform: translateY(-5px);
        }

        .skill-card h3 {
            color: #2c3e50;
            margin-bottom: 10px;
        }

        .contact-info {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 10px;
            margin-top: 30px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }

        .contact-item i {
            font-size: 1.5rem;
            color: #667eea;
            margin-right: 15px;
            width: 30px;
        }

        footer {
            text-align: center;
            padding: 30px;
            color: white;
            margin-top: 40px;
        }

        .ethiopia-flag {
            color: #FFD700;
            font-weight: bold;
        }

        /* If image doesn't load, show text fallback */
        .logo-fallback {
            display: none;
            font-size: 3rem;
            font-weight: bold;
            color: #2c3e50;
        }

        .logo-fallback .grah {
            color: #667eea;
        }

        .logo-fallback .web {
            color: #764ba2;
            font-size: 4rem;
        }

        .logo-fallback .dev {
            color: #FFD700;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo-container">
                <!-- Replace 'your-logo.png' with your actual image file name -->
                <img src="1000015911.png" alt="GRAH WEB DEVELOPMENT" class="logo-image" onerror="this.style.display='none'; document.getElementById('fallback').style.display='block';">
                <div id="fallback" class="logo-fallback">
                    <span class="grah">GRAH</span><br>
                    <span class="web">WEB</span><br>
                    <span class="dev">DEVELOPMENT</span>
                </div>
            </div>
            <div class="tagline">Building the Future with Code</div>
        </header>

        <div class="main-content">
            <section class="profile-section">
                <div class="profile-image">MS</div>
                <div class="profile-info">
                    <h1>Mesud Seid</h1>
                    <p class="university">First Year Computer Science Student</p>
                    <p class="university">Wollo University, Ethiopia</p>
                    
                    <div class="goal">
                        <p>I am passionate about technology and currently on a journey to become a great Ethiopian programmer. I believe in the power of code to transform lives and communities.</p>
                    </div>
                </div>
            </section>

            <section class="about">
                <h2>My Journey</h2>
                <p>As a first-year Computer Science student at Wollo University, I'm building my foundation in programming fundamentals, algorithms, and software development principles.</p>
                <p>My goal is to master web development technologies and contribute to Ethiopia's growing tech ecosystem. I'm particularly interested in creating solutions that address local challenges.</p>
            </section>

            <section class="skills-section">
                <h2>Skills & Interests</h2>
                <div class="skills">
                    <div class="skill-card">
                        <h3>Web Development</h3>
                        <p>HTML, CSS, JavaScript</p>
                    </div>
                    <div class="skill-card">
                        <h3>Programming</h3>
                        <p>C++, Python, Java</p>
                    </div>
                    <div class="skill-card">
                        <h3>Problem Solving</h3>
                        <p>Algorithms & Data Structures</p>
                    </div>
                    <div class="skill-card">
                        <h3>Ethiopian Tech</h3>
                        <p>Local solutions for local challenges</p>
                    </div>
                </div>
            </section>

            <section class="contact">
                <h2>Get In Touch</h2>
                <div class="contact-info">
                    <div class="contact-item">
                        <i>📧</i>
                        <span>Email: mesud.seid@example.com</span>
                    </div>
                    <div class="contact-item">
                        <i>🏫</i>
                        <span>University: Wollo University</span>
                    </div>
                    <div class="contact-item">
                        <i>📍</i>
                        <span>Location: Ethiopia</span>
                    </div>
                    <div class="contact-item">
                        <i>🌐</i>
                        <span>Website: me14se.github.io/mesud-personal-web-site</span>
                    </div>
                </div>
            </section>
        </div>

        <footer>
            <p>&copy; 2024 Mesud Seid. All rights reserved.</p>
            <p>Proudly Ethiopian <span class="ethiopia-flag">🇪🇹</span> | GRAH WEB DEVELOPMENT</p>
        </footer>
    </div>

    <script>
        // Simple script to handle image loading
        document.addEventListener('DOMContentLoaded', function() {
            const logoImg = document.querySelector('.logo-image');
            const fallback = document.getElementById('fallback');
            
            // Check if image loaded successfully
            if (logoImg.complete && logoImg.naturalHeight === 0) {
                fallback.style.display = 'block';
            }
        });
    </script>
</body>
</html>
