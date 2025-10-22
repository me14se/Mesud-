<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mesud Seid - Ethiopian Programmer & Content Creator</title>
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

        .logo-fallback {
            font-size: 3rem;
            font-weight: bold;
            color: #2c3e50;
            text-align: center;
        }

        .logo-fallback .grah { color: #667eea; }
        .logo-fallback .web { color: #764ba2; font-size: 4rem; }
        .logo-fallback .dev { color: #FFD700; }

        .tagline {
            font-size: 1.3rem;
            margin-bottom: 30px;
            opacity: 0.9;
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

        h3 {
            color: #2c3e50;
            margin: 20px 0 10px;
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

        /* Social Media Styles */
        .social-media {
            margin: 30px 0;
        }

        .social-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .social-card {
            background: white;
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
            border: 2px solid transparent;
        }

        .social-card:hover {
            transform: translateY(-5px);
        }

        .social-card.tiktok { border-color: #000000; }
        .social-card.youtube { border-color: #FF0000; }
        .social-card.instagram { 
            border-color: transparent;
            background: linear-gradient(45deg, #405DE6, #5851DB, #833AB4, #C13584, #E1306C, #FD1D1D);
            color: white;
        }
        .social-card.linkedin { border-color: #0077B5; }

        .social-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
        }

        .social-card h3 {
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .social-card a {
            display: inline-block;
            background: #667eea;
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            margin-top: 10px;
            transition: background 0.3s ease;
            font-weight: bold;
        }

        .social-card a:hover {
            background: #764ba2;
            transform: scale(1.05);
        }

        /* Video Section */
        .video-section {
            margin: 40px 0;
        }

        .video-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 30px 0;
        }

        .video-card {
            background: #f8f9fa;
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .video-card:hover {
            transform: translateY(-5px);
        }

        .video-container {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            margin-bottom: 15px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        .video-info {
            text-align: center;
        }

        .video-info h4 {
            color: #2c3e50;
            margin-bottom: 10px;
            font-size: 1.2rem;
        }

        .video-info p {
            color: #666;
            font-size: 0.9rem;
        }

        /* Interactive Gallery */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }

        .gallery-item {
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            background: #f8f9fa;
            height: 200px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #667eea;
            font-weight: bold;
            transition: transform 0.3s ease;
            position: relative;
            cursor: pointer;
            flex-direction: column;
            text-align: center;
            padding: 20px;
        }

        .gallery-item:hover {
            transform: scale(1.05);
            background: #667eea;
            color: white;
        }

        .gallery-item.active {
            background: #764ba2;
            color: white;
            transform: scale(1.02);
        }

        .gallery-icon {
            font-size: 3rem;
            margin-bottom: 10px;
        }

        .description-panel {
            background: #f8f9fa;
            padding: 0;
            border-radius: 15px;
            margin-top: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            max-height: 0;
            overflow: hidden;
            transition: all 0.5s ease;
        }

        .description-panel.active {
            padding: 30px;
            max-height: 500px;
        }

        .description-content h3 {
            color: #2c3e50;
            margin-bottom: 15px;
            border-bottom: 2px solid #667eea;
            padding-bottom: 10px;
        }

        .description-content p {
            margin-bottom: 15px;
            line-height: 1.8;
        }

        .struggle-list {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            margin: 15px 0;
            border-left: 4px solid #FFD700;
        }

        .struggle-list li {
            margin-bottom: 10px;
            padding-left: 10px;
        }

        .follower-count {
            font-size: 0.9rem;
            color: #666;
            margin-top: 5px;
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

        .stats {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .stat-item {
            background: rgba(255,255,255,0.1);
            padding: 15px 25px;
            border-radius: 10px;
            text-align: center;
        }

        .stat-number {
            font-size: 1.5rem;
            font-weight: bold;
            color: #FFD700;
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

        .contact-item span:first-child {
            font-size: 1.5rem;
            margin-right: 15px;
            width: 30px;
        }

        .platform-badge {
            display: inline-block;
            background: #667eea;
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
            margin-left: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo-container">
                <div class="logo-fallback">
                    <span class="grah">welcome</span><br>
                    <span class="web">WEB</span><br>
                    <span class="dev">DEVELOPMENT</span>
                </div>
            </div>
            <div class="tagline">Building the Future with Code & Content</div>
            
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">3</div>
                    <div>Platforms</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">2</div>
                    <div>Videos</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">🇪🇹</div>
                    <div>Ethiopian</div>
                </div>
            </div>
        </header>

        <div class="main-content">
            <section class="profile-section">
                <div class="profile-image">MS</div>
                <div class="profile-info">
                    <h1>Mesud Seid</h1>
                    <p class="university">First Year Computer Science Student</p>
                    <p class="university">Wollo University, Ethiopia</p>
                    
                    <div class="goal">
                        <p>I create programming content and tutorials while building my skills as a developer. Check out my latest videos and follow my journey across all platforms!</p>
                    </div>
                </div>
            </section>

            <!-- Video Gallery Section -->
            <section class="video-section">
                <h2>My Latest Videos</h2>
                <p>Watch my programming content across different platforms:</p>
                
                <div class="video-gallery">
                    <!-- TikTok Video -->
                    <div class="video-card">
                        <div class="video-container">
                            <!-- TikTok Embed -->
                            <iframe src="https://www.tiktok.com/embed/v2/MAV3q7Xv" 
                                    title="TikTok Video"
                                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                    allowfullscreen>
                            </iframe>
                        </div>
                        <div class="video-info">
                            <h4>Programming on TikTok <span class="platform-badge">TikTok</span></h4>
                            <p>Short programming tips and coding content</p>
                            <a href="https://vm.tiktok.com/ZMAV3q7Xv/" target="_blank" style="color: #667eea; text-decoration: none;">▶ Watch on TikTok</a>
                        </div>
                    </div>

                    <!-- YouTube Short -->
                    <div class="video-card">
                        <div class="video-container">
                            <!-- YouTube Short Embed -->
                            <iframe src="https://www.youtube.com/embed/e0pZyOdhl-8" 
                                    title="YouTube Short"
                                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                    allowfullscreen>
                            </iframe>
                        </div>
                        <div class="video-info">
                            <h4>YouTube Short <span class="platform-badge">YouTube</span></h4>
                            <p>Quick programming insights and tutorials</p>
                            <a href="https://youtube.com/shorts/e0pZyOdhl-8?si=harpPRTa9vhRWzXV" target="_blank" style="color: #667eea; text-decoration: none;">▶ Watch on YouTube</a>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Interactive Gallery Section -->
            <section class="gallery-section">
                <h2>My Journey & Vision</h2>
                <p>Click on each section to learn more about my journey:</p>
                
                <div class="gallery">
                    <div class="gallery-item" onclick="showDescription('coding')">
                        <div class="gallery-icon">💻</div>
                        <div>Coding Projects</div>
                    </div>
                    <div class="gallery-item" onclick="showDescription('university')">
                        <div class="gallery-icon">🎓</div>
                        <div>University Life</div>
                    </div>
                    <div class="gallery-item" onclick="showDescription('future')">
                        <div class="gallery-icon">🚀</div>
                        <div>Future Goals</div>
                    </div>
                    <div class="gallery-item" onclick="showDescription('ethiopia')">
                        <div class="gallery-icon">🇪🇹</div>
                        <div>Ethiopian Tech</div>
                    </div>
                </div>

                <!-- Description Panel -->
                <div class="description-panel" id="descriptionPanel">
                    <div class="description-content" id="descriptionContent">
                        <!-- Content will be inserted here by JavaScript -->
                    </div>
                </div>
            </section>

            <!-- Social Media Section -->
            <section class="social-media">
                <h2>Follow My Programming Journey</h2>
                <p>Join me across platforms for different types of content - from short tips to full tutorials!</p>
                
                <div class="social-grid">
                    <div class="social-card tiktok">
                        <div class="social-icon">📱</div>
                        <h3>TikTok</h3>
                        <p>Short programming videos & quick tips</p>
                        <p class="follower-count">Username: @m.1love1</p>
                        <a href="https://tiktok.com/@m.1love1" target="_blank">Follow on TikTok</a>
                    </div>
                    
                    <div class="social-card youtube">
                        <div class="social-icon">📺</div>
                        <h3>YouTube</h3>
                        <p>Full programming tutorials & projects</p>
                        <p class="follower-count">@mesudtech Channel</p>
                        <a href="https://youtube.com/@mesudtech?si=WQqg5_07e3JdUy9Q" target="_blank">Subscribe on YouTube</a>
                    </div>
                    
                    <div class="social-card instagram">
                        <div class="social-icon">📷</div>
                        <h3>Instagram</h3>
                        <p>Daily coding journey & behind the scenes</p>
                        <p class="follower-count">@mesud11sei</p>
                        <a href="https://www.instagram.com/mesud11sei?igsh=bGxhZGduOXYzNW12" target="_blank">Follow on Instagram</a>
                    </div>
                    
                    <div class="social-card linkedin">
                        <div class="social-icon">💼</div>
                        <h3>Professional</h3>
                        <p>Connect for career opportunities</p>
                        <p class="follower-count">Let's network</p>
                        <a href="https://linkedin.com/in/yourprofile" target="_blank">Connect on LinkedIn</a>
                    </div>
                </div>
            </section>

            <!-- Call to Action -->
            <section class="goal" style="text-align: center; margin: 40px 0;">
                <h3>Let's Grow Together! 🌱</h3>
                <p>Follow me on all platforms to join my journey from CS student to professional developer.</p>
                <p>I share programming tips, project walkthroughs, and daily learning experiences!</p>
                <div style="margin-top: 20px;">
                    <a href="https://tiktok.com/@m.1love1" style="background: #000; color: white; padding: 12px 25px; border-radius: 25px; text-decoration: none; margin: 5px;">Follow on TikTok</a>
                    <a href="https://youtube.com/@mesudtech" style="background: #FF0000; color: white; padding: 12px 25px; border-radius: 25px; text-decoration: none; margin: 5px;">Subscribe on YouTube</a>
                </div>
            </section>

            <section class="contact">
                <h2>Get In Touch</h2>
                <div class="contact-info">
                    <div class="contact-item">
                        <span>📧</span>
                        <span>Email: mesud.seid@example.com</span>
                    </div>
                    <div class="contact-item">
                        <span>🏫</span>
                        <span>University: Wollo University</span>
                    </div>
                    <div class="contact-item">
                        <span>📍</span>
                        <span>Location: Ethiopia 🇪🇹</span>
                    </div>
                    <div class="contact-item">
                        <span>🌐</span>
                        <span>Website: me14se.github.io/mesud-personal-web-site</span>
                    </div>
                </div>
            </section>
        </div>

        <footer>
            <p>&copy; 2025 Mesud Seid. All rights reserved.</p>
            <p>Proudly Ethiopian <span class="ethiopia-flag">🇪🇹</span> | Content Creator & Programmer</p>
            <p>Watch my videos and follow my programming journey! 🚀</p>
            <div style="margin-top: 15px;">
                <a href="https://tiktok.com/@m.1love1" style="color: #FFD700; margin: 0 10px;">TikTok</a> •
                <a href="https://youtube.com/@mesudtech" style="color: #FFD700; margin: 0 10px;">YouTube</a> •
                <a href="https://instagram.com/mesud11sei" style="color: #FFD700; margin: 0 10px;">Instagram</a>
            </div>
        </footer>
    </div>

    <script>
        // Description content
        const descriptions = {
            coding: {
                title: "My Coding Projects",
                content: `
                    <p>I'm currently working on several programming projects to build my skills:</p>
                    <div class="struggle-list">
                        <h4>Current Projects:</h4>
                        <ul>
                            <li><strong>Personal Website:</strong> This very website you're browsing! Built with HTML, CSS, and JavaScript</li>
                            <li><strong>Python Automation:</strong> Creating scripts to automate daily tasks and improve productivity</li>
                            <li><strong>Mobile Apps:</strong> Learning React Native to build cross-platform mobile applications</li>
                            <li><strong>Ethiopian Tech Solutions:</strong> Working on ideas that solve local problems in Ethiopia</li>
                        </ul>
                    </div>
                    <p>Every day I'm learning new technologies and pushing myself to become a better programmer. The journey is challenging but incredibly rewarding!</p>
                `
            },
            university: {
                title: "University Life & Struggles",
                content: `
                    <p>Being a first-year Computer Science student at Wollo University comes with its own set of challenges and learning experiences:</p>
                    <div class="struggle-list">
                        <h4>My Daily Struggles:</h4>
                        <ul>
                            <li><strong>Limited Resources:</strong> Learning advanced programming with basic equipment</li>
                            <li><strong>Internet Challenges:</strong> Dealing with connectivity issues while trying to access online resources</li>
                            <li><strong>Balancing Studies:</strong> Juggling between theoretical courses and practical coding practice</li>
                            <li><strong>Self-Learning:</strong> Going beyond classroom materials to learn modern technologies</li>
                            <li><strong>Time Management:</strong> Balancing university assignments with personal projects</li>
                        </ul>
                    </div>
                    <p>Despite these challenges, I'm determined to succeed. Every obstacle makes me stronger and more creative in finding solutions!</p>
                `
            },
            future: {
                title: "My Future Goals & Vision",
                content: `
                    <p>I have big dreams for my future in technology and programming:</p>
                    <div class="struggle-list">
                        <h4>My 5-Year Vision:</h4>
                        <ul>
                            <li><strong>Become Full-Stack Developer:</strong> Master both frontend and backend technologies</li>
                            <li><strong>Build Ethiopian Tech Startup:</strong> Create solutions that address local challenges in Ethiopia</li>
                            <li><strong>Grow My Online Presence:</strong> Reach 100,000+ followers across my social media platforms</li>
                            <li><strong>Mentor Other Students:</strong> Help other Ethiopian students learn programming</li>
                            <li><strong>International Opportunities:</strong> Work with global tech companies while representing Ethiopia</li>
                        </ul>
                    </div>
                    <p>I believe that with consistent effort and learning, I can achieve these goals and make a positive impact in the tech community!</p>
                `
            },
            ethiopia: {
                title: "Ethiopian Technology Vision",
                content: `
                    <p>I'm passionate about contributing to Ethiopia's growing tech ecosystem:</p>
                    <div class="struggle-list">
                        <h4>My Focus Areas for Ethiopia:</h4>
                        <ul>
                            <li><strong>Local Solutions:</strong> Developing apps and software that solve Ethiopian-specific problems</li>
                            <li><strong>Tech Education:</strong> Creating programming content in Amharic and local languages</li>
                            <li><strong>Digital Transformation:</strong> Helping traditional businesses adopt technology</li>
                            <li><strong>Youth Empowerment:</strong> Inspiring the next generation of Ethiopian programmers</li>
                            <li><strong>Global Representation:</strong> Putting Ethiopian developers on the world map</li>
                        </ul>
                    </div>
                    <p>I dream of a future where Ethiopia is known for innovation and technology, not just our rich history and culture. The youth have the power to make this happen!</p>
                `
            }
        };

        function showDescription(type) {
            const panel = document.getElementById('descriptionPanel');
            const content = document.getElementById('descriptionContent');
            const items = document.querySelectorAll('.gallery-item');
            
            // Remove active class from all items
            items.forEach(item => item.classList.remove('active'));
            
            // Add active class to clicked item
            event.currentTarget.classList.add('active');
            
            // Update content
            content.innerHTML = `
                <h3>${descriptions[type].title}</h3>
                ${descriptions[type].content}
            `;
            
            // Show panel with animation
            panel.classList.add('active');
        }

        // Simple animation for cards
        document.addEventListener('DOMContentLoaded', function() {
            const cards = document.querySelectorAll('.social-card, .video-card, .gallery-item');
            
            cards.forEach((card, index) => {
                card.style.animationDelay = `${index * 0.1}s`;
            });
        });
    </script>
</body>
</html>
