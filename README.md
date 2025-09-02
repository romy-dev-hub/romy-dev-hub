<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roumaissa Hadibi | GitHub README</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: #0a0a0a;
            color: #fff;
            line-height: 1.6;
            padding: 20px;
            max-width: 900px;
            margin: 0 auto;
        }
        
        .container {
            background: linear-gradient(135deg, #0f0f1a 0%, #1a1a2e 100%);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            border: 1px solid #2d2d4d;
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
            padding: 20px 0;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: linear-gradient(45deg, #8a2be2, #ff3e7f);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: fadeIn 1s ease-out;
        }
        
        .title {
            font-size: 1.2rem;
            color: #a0a0d0;
            margin-bottom: 20px;
            animation: slideUp 1s ease-out;
        }
        
        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, #8a2be2, #ff3e7f, transparent);
            margin: 25px 0;
            border: none;
            animation: expand 1.5s ease-out;
        }
        
        section {
            margin-bottom: 30px;
            opacity: 0;
            animation: fadeIn 0.8s forwards;
        }
        
        section:nth-child(1) { animation-delay: 0.2s; }
        section:nth-child(2) { animation-delay: 0.4s; }
        section:nth-child(3) { animation-delay: 0.6s; }
        section:nth-child(4) { animation-delay: 0.8s; }
        section:nth-child(5) { animation-delay: 1.0s; }
        
        h2 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #8a2be2;
            display: flex;
            align-items: center;
        }
        
        h2 i {
            margin-right: 10px;
            color: #ff3e7f;
        }
        
        p {
            margin-bottom: 15px;
            color: #d0d0e7;
        }
        
        .highlight {
            color: #ff3e7f;
            font-weight: 500;
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            gap: 12px;
            margin-top: 15px;
        }
        
        .tech-item {
            background: rgba(138, 43, 226, 0.1);
            padding: 10px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s, background 0.3s;
            border: 1px solid rgba(138, 43, 226, 0.3);
        }
        
        .tech-item:hover {
            transform: translateY(-5px);
            background: rgba(138, 43, 226, 0.2);
        }
        
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 15px;
        }
        
        .project-card {
            background: rgba(26, 26, 46, 0.7);
            border-radius: 10px;
            padding: 15px;
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid rgba(255, 62, 127, 0.2);
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(255, 62, 127, 0.2);
        }
        
        .project-card h3 {
            color: #ff3e7f;
            margin-bottom: 10px;
            font-size: 1.1rem;
        }
        
        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        .contact-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            background: rgba(138, 43, 226, 0.1);
            border-radius: 50%;
            color: #ff3e7f;
            font-size: 1.5rem;
            transition: transform 0.3s, background 0.3s;
            border: 1px solid rgba(138, 43, 226, 0.3);
            text-decoration: none;
        }
        
        .contact-link:hover {
            transform: scale(1.1);
            background: rgba(138, 43, 226, 0.2);
        }
        
        .quote {
            text-align: center;
            font-style: italic;
            color: #a0a0d0;
            margin-top: 30px;
            padding: 15px;
            border-top: 1px solid rgba(255, 62, 127, 0.3);
            border-bottom: 1px solid rgba(255, 62, 127, 0.3);
            animation: pulse 2s infinite;
        }
        
        .badge {
            display: inline-block;
            padding: 4px 8px;
            border-radius: 4px;
            font-size: 0.8rem;
            margin: 0 5px 5px 0;
            background: rgba(255, 62, 127, 0.2);
            color: #ff9ec5;
            border: 1px solid rgba(255, 62, 127, 0.3);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { transform: translateY(20px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        @keyframes expand {
            from { width: 0%; margin: 0 auto; }
            to { width: 100%; margin: 25px 0; }
        }
        
        @keyframes pulse {
            0% { opacity: 0.8; }
            50% { opacity: 1; }
            100% { opacity: 0.8; }
        }
        
        @media (max-width: 768px) {
            .tech-grid {
                grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
            }
            
            .project-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Hi, I'm Xiao ro! 👋</h1>
            <p class="title">💻 Front-End & Games Developer | 🎙️ Podcaster | 🌿 Nature Lover | 🚀 Future AI Engineer</p>
        </header>
        
        <hr class="divider">
        
        <section id="about">
            <h2><i class="fas fa-user"></i> About Me</h2>
            <p>I'm a passionate <span class="highlight">2nd-year Computer Science student</span> at USTHB with a love for creating beautiful and functional digital experiences.</p>
            <p>🎮 I've developed <span class="highlight"> games in Python, Java, C and Lua</span>, combining logic with creative gameplay.</p>
            <p>🌱 Currently mastering <span class="highlight">JavaScript, React, and UI/UX design</span> principles.</p>
            <p>🎙️ Creator and host of the <span class="highlight">Legacy Podcast</span>, where we share meaningful stories that resonate.</p>
            <p>🌿 In my ideal world, I'm coding from a peaceful cabin surrounded by nature.</p>
        </section>
        
        <hr class="divider">
        
        <section id="tech-stack">
            <h2><i class="fas fa-code"></i> Tech Stack</h2>
            <div class="tech-grid">
                <div class="tech-item">Java</div>
                <div class="tech-item">JavaFX</div>
                <div class="tech-item">Oracle SQL</div>
                <div class="tech-item">Python</div>
                <div class="tech-item">C</div>
                <div class="tech-item">HTML5</div>
                <div class="tech-item">CSS3</div>
                <div class="tech-item">JavaScript</div>
                <div class="tech-item">React.js</div>
                <div class="tech-item">Git</div>
                <div class="tech-item">TypeScript</div>
                <div class="tech-item">Next.js</div>
                <div class="tech-item">Three.js</div>
            </div>
        </section>
        
        <hr class="divider">
        
        <section id="projects">
            <h2><i class="fas fa-laptop-code"></i> Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <h3>Pixelspark</h3>
                    <p>A beautifully designed food website with clean UI and excellent user experience.</p>
                    <span class="badge">HTML</span>
                    <span class="badge">CSS</span>
                    <span class="badge">JavaScript</span>
                </div>
                <div class="project-card">
                    <h3>Legacy Podcast</h3>
                    <p>A platform for sharing impactful stories and conversations (coming soon).</p>
                    <span class="badge">React</span>
                    <span class="badge">Audio</span>
                    <span class="badge">UI/UX</span>
                </div>
                <div class="project-card">
                    <h3>Python Games</h3>
                    <p>Two engaging games built with Python, showcasing gameplay mechanics and logic.</p>
                    <span class="badge">Python</span>
                    <span class="badge">Game Dev</span>
                </div>
                <div class="project-card">
                    <h3>C Game</h3>
                    <p>A low-level game development project demonstrating C programming skills.</p>
                    <span class="badge">C</span>
                    <span class="badge">Game Dev</span>
                </div>
                <div class="project-card">
                    <h3>Library Management</h3>
                    <p>A full-stack application for managing library resources with JavaFX and Oracle.</p>
                    <span class="badge">Java</span>
                    <span class="badge">JavaFX</span>
                    <span class="badge">Oracle SQL</span>
                </div>
            </div>
        </section>
        
        <hr class="divider">
        
        <section id="contact">
            <h2><i class="fas fa-envelope"></i> Let's Connect</h2>
            <p>I'm always open to discussing new projects, creative ideas, or opportunities to be part of your vision.</p>
            
            <div class="contact-links">
                <a href="mailto:roumaissa.hadibi.dev@gmail.com" class="contact-link">
                    <i class="fas fa-envelope"></i>
                </a>
                <a href="https://github.com/romy-dev-hub" class="contact-link">
                    <i class="fab fa-github"></i>
                </a>
                <a href="https://xiao-ro-portfolio.vercel.app/" class="contact-link">
                    <i class="fas fa-globe"></i>
                </a>
            </div>
            
            <p style="text-align: center; margin-top: 15px;">
                <i class="fab fa-discord"></i> Discord: sayonara_romy
            </p>
        </section>
        
        <p class="quote">"Code is my language. Legacy is my voice. The world is my canvas."</p>
    </div>

    <script>
        // Simple intersection observer for animations
        document.addEventListener('DOMContentLoaded', function() {
            const sections = document.querySelectorAll('section');
            
            sections.forEach(section => {
                section.style.opacity = '1';
            });
        });
    </script>
</body>
</html>