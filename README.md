<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dilsha Perera | QA Engineer</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        :root {
            --primary: #6C63FF;
            --secondary: #FF6584;
            --accent: #43B02A;
            --dark: #2D2B55;
            --light: #F5F5F7;
            --gradient: linear-gradient(135deg, #6C63FF 0%, #FF6584 100%);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background-color: #0F0F23;
            color: var(--light);
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        /* Header Styles */
        .header {
            text-align: center;
            padding: 4rem 0;
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(108, 99, 255, 0.1) 0%, rgba(0, 0, 0, 0) 70%);
            z-index: -1;
            animation: pulse 8s infinite alternate;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); opacity: 0.5; }
            100% { transform: scale(1.1); opacity: 0.8; }
        }
        
        .name {
            font-size: 3.5rem;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 1rem;
            animation: fadeInDown 1s ease;
            font-weight: 700;
        }
        
        .title {
            font-size: 1.8rem;
            margin-bottom: 0.5rem;
            color: var(--light);
            animation: fadeInUp 1s ease 0.2s both;
            font-weight: 500;
        }
        
        .subtitle {
            font-size: 1.2rem;
            color: #A0A0C0;
            animation: fadeInUp 1s ease 0.4s both;
            margin-bottom: 2rem;
        }
        
        /* Intro Section */
        .intro {
            text-align: center;
            padding: 2rem 0;
            margin: 2rem 0;
            background: rgba(45, 43, 85, 0.5);
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(108, 99, 255, 0.2);
            animation: fadeIn 1s ease 0.6s both;
            position: relative;
            overflow: hidden;
        }
        
        .intro::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(108, 99, 255, 0.1), transparent);
            animation: shimmer 3s infinite;
        }
        
        @keyframes shimmer {
            0% { left: -100%; }
            100% { left: 100%; }
        }
        
        .intro p {
            margin: 0.5rem 0;
            font-size: 1.1rem;
        }
        
        .highlight {
            color: var(--secondary);
            font-weight: 600;
        }
        
        .email {
            color: var(--primary);
            text-decoration: none;
            transition: all 0.3s ease;
            font-weight: 500;
        }
        
        .email:hover {
            color: var(--secondary);
            text-shadow: 0 0 10px rgba(255, 101, 132, 0.5);
        }
        
        /* Section Headers */
        .section-header {
            text-align: center;
            margin: 3rem 0 2rem;
            position: relative;
        }
        
        .section-header h2 {
            font-size: 2.2rem;
            display: inline-block;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            position: relative;
            padding-bottom: 10px;
        }
        
        .section-header h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: var(--gradient);
            border-radius: 2px;
        }
        
        /* Social Links */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }
        
        .social-link {
            display: inline-flex;
            align-items: center;
            padding: 0.8rem 1.5rem;
            background: rgba(45, 43, 85, 0.7);
            border-radius: 50px;
            text-decoration: none;
            color: var(--light);
            font-weight: 500;
            transition: all 0.3s ease;
            border: 1px solid rgba(108, 99, 255, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .social-link::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: var(--gradient);
            transition: all 0.5s ease;
            z-index: -1;
        }
        
        .social-link:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(108, 99, 255, 0.3);
            color: white;
        }
        
        .social-link:hover::before {
            left: 0;
        }
        
        .social-link img {
            margin-right: 8px;
            filter: brightness(0) invert(1);
            width: 20px;
            height: 20px;
        }
        
        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }
        
        .skill-item {
            background: rgba(45, 43, 85, 0.7);
            border-radius: 15px;
            padding: 1.5rem 1rem;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(108, 99, 255, 0.2);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
        }
        
        .skill-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: var(--gradient);
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.3s ease;
        }
        
        .skill-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
        }
        
        .skill-item:hover::before {
            transform: scaleX(1);
        }
        
        .skill-item img {
            width: 40px;
            height: 40px;
            margin-bottom: 10px;
            filter: brightness(0.8);
            transition: all 0.3s ease;
        }
        
        .skill-item:hover img {
            filter: brightness(1);
            transform: scale(1.1);
        }
        
        .skill-item .badge {
            background: var(--gradient);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
            margin-top: 5px;
        }
        
        /* Projects Section */
        .projects-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }
        
        .project-card {
            background: rgba(45, 43, 85, 0.7);
            border-radius: 20px;
            padding: 2rem;
            transition: all 0.3s ease;
            border: 1px solid rgba(108, 99, 255, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .project-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient);
            opacity: 0;
            transition: all 0.3s ease;
            z-index: -1;
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
        }
        
        .project-card:hover::before {
            opacity: 0.1;
        }
        
        .project-icon {
            font-size: 2rem;
            margin-bottom: 1rem;
        }
        
        .project-title {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: var(--light);
        }
        
        .project-desc {
            color: #A0A0C0;
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }
        
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1.5rem;
        }
        
        .tech-tag {
            background: rgba(108, 99, 255, 0.2);
            color: var(--primary);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
        }
        
        .project-link {
            display: inline-block;
            padding: 0.7rem 1.5rem;
            background: var(--gradient);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        .project-link:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(108, 99, 255, 0.4);
        }
        
        /* Stats Section */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }
        
        .stat-card {
            background: rgba(45, 43, 85, 0.7);
            border-radius: 20px;
            padding: 2rem;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(108, 99, 255, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .stat-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient);
            opacity: 0;
            transition: all 0.3s ease;
            z-index: -1;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .stat-card:hover::before {
            opacity: 0.1;
        }
        
        .stat-title {
            font-size: 1rem;
            color: #A0A0C0;
            margin-bottom: 1rem;
        }
        
        .stat-value {
            font-size: 2.5rem;
            font-weight: 700;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        /* Highlights Section */
        .highlights {
            background: rgba(45, 43, 85, 0.7);
            border-radius: 20px;
            padding: 2.5rem;
            margin: 3rem 0;
            border: 1px solid rgba(108, 99, 255, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .highlights::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255, 101, 132, 0.1) 0%, rgba(0, 0, 0, 0) 70%);
            z-index: -1;
            animation: pulse 6s infinite alternate-reverse;
        }
        
        .highlights h3 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 1.8rem;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .highlight-list {
            list-style: none;
        }
        
        .highlight-item {
            padding: 1rem 0;
            border-bottom: 1px solid rgba(108, 99, 255, 0.2);
            display: flex;
            align-items: center;
        }
        
        .highlight-item:last-child {
            border-bottom: none;
        }
        
        .highlight-icon {
            margin-right: 1rem;
            font-size: 1.5rem;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        /* Footer */
        .footer {
            text-align: center;
            padding: 3rem 0 2rem;
            color: #A0A0C0;
            font-size: 0.9rem;
            position: relative;
        }
        
        .footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 200px;
            height: 3px;
            background: var(--gradient);
            border-radius: 2px;
        }
        
        .signature {
            margin-top: 1rem;
            font-size: 1rem;
            color: var(--light);
        }
        
        .heart {
            color: var(--secondary);
            animation: heartbeat 1.5s infinite;
            display: inline-block;
        }
        
        @keyframes heartbeat {
            0% { transform: scale(1); }
            5% { transform: scale(1.1); }
            10% { transform: scale(1); }
            15% { transform: scale(1.1); }
            20% { transform: scale(1); }
            100% { transform: scale(1); }
        }
        
        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* Floating Elements */
        .floating {
            position: absolute;
            width: 50px;
            height: 50px;
            background: rgba(108, 99, 255, 0.1);
            border-radius: 50%;
            animation: float 6s ease-in-out infinite;
            z-index: -1;
        }
        
        .floating:nth-child(1) {
            top: 10%;
            left: 10%;
            width: 30px;
            height: 30px;
            animation-delay: 0s;
        }
        
        .floating:nth-child(2) {
            top: 20%;
            right: 15%;
            width: 40px;
            height: 40px;
            animation-delay: 1s;
        }
        
        .floating:nth-child(3) {
            bottom: 20%;
            left: 15%;
            width: 35px;
            height: 35px;
            animation-delay: 2s;
        }
        
        .floating:nth-child(4) {
            bottom: 10%;
            right: 10%;
            width: 45px;
            height: 45px;
            animation-delay: 3s;
        }
        
        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
            100% { transform: translateY(0) rotate(360deg); }
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .name {
                font-size: 2.5rem;
            }
            
            .title {
                font-size: 1.5rem;
            }
            
            .subtitle {
                font-size: 1rem;
            }
            
            .skills-container {
                grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
            }
            
            .projects-container {
                grid-template-columns: 1fr;
            }
            
            .social-links {
                flex-direction: column;
                align-items: center;
            }
            
            .social-link {
                width: 200px;
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Floating Elements -->
        <div class="floating"></div>
        <div class="floating"></div>
        <div class="floating"></div>
        <div class="floating"></div>
        
        <!-- Header Section -->
        <div class="header">
            <h1 class="name">Hi 👋, I'm Dilsha Perera</h1>
            <h2 class="title">Aspiring QA Engineer | Software Testing Enthusiast | Manual & Automation Testing</h2>
            <h3 class="subtitle">A passionate Software Engineering Student from Sri Lanka</h3>
        </div>
        
        <!-- Intro Section -->
        <div class="intro">
            <p>🌱 I'm currently learning <span class="highlight">Selenium, Jira</span></p>
            <p>💼 Looking to contribute to real-world QA projects and gain hands-on experience</p>
            <p>📫 Reach me at: <a href="mailto:dilshaperera1118@gmail.com" class="email">dilshaperera1118@gmail.com</a></p>
        </div>
        
        <!-- Connect Section -->
        <div class="section-header">
            <h2>Connect with me</h2>
        </div>
        
        <div class="social-links">
            <a href="https://linkedin.com/in/dilsha-perera" target="_blank" class="social-link">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/linkedin.svg" alt="LinkedIn">
                LinkedIn
            </a>
            <a href="https://facebook.com/dilsha.perera" target="_blank" class="social-link">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/facebook.svg" alt="Facebook">
                Facebook
            </a>
            <a href="https://instagram.com/dilsha.perera" target="_blank" class="social-link">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/instagram.svg" alt="Instagram">
                Instagram
            </a>
        </div>
        
        <!-- Skills Section -->
        <div class="section-header">
            <h2>Skills & Tools</h2>
        </div>
        
        <div class="skills-container">
            <div class="skill-item">
                <img src="https://cdn.worldvectorlogo.com/logos/figma-1.svg" alt="Figma">
                <span>Figma</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/spring.svg" alt="Spring Boot">
                <span>Spring Boot</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/intellijidea.svg" alt="IntelliJ IDEA">
                <span>IntelliJ IDEA</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/webstorm.svg" alt="WebStorm">
                <span>WebStorm</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/visualstudiocode.svg" alt="VS Code">
                <span>VS Code</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/postman.svg" alt="Postman">
                <span>Postman</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/selenium.svg" alt="Selenium">
                <span>Selenium</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/java.svg" alt="Java">
                <span>Java</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/python.svg" alt="Python">
                <span>Python</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/mysql.svg" alt="MySQL">
                <span>MySQL</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/mongodb.svg" alt="MongoDB">
                <span>MongoDB</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/git.svg" alt="Git">
                <span>Git</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/github.svg" alt="GitHub">
                <span>GitHub</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/html5.svg" alt="HTML5">
                <span>HTML5</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/css3.svg" alt="CSS3">
                <span>CSS3</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/javascript.svg" alt="JavaScript">
                <span>JavaScript</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/linux.svg" alt="Linux">
                <span>Linux</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/arduino.svg" alt="Arduino">
                <span>Arduino</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/apachejmeter.svg" alt="JMeter">
                <span>JMeter</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/jira.svg" alt="Jira">
                <span>Jira</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/react.svg" alt="React Native">
                <span>React Native</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/apachetomcat.svg" alt="Tomcat">
                <span>Tomcat</span>
            </div>
            <div class="skill-item">
                <img src="https://cdn.jsdelivr.net/npm/simple-icons@v5/icons/hibernate.svg" alt="Hibernate">
                <span>Hibernate</span>
            </div>
        </div>
        
        <!-- Projects Section -->
        <div class="section-header">
            <h2>Projects</h2>
        </div>
        
        <div class="projects-container">
            <div class="project-card">
                <div class="project-icon">🩸</div>
                <h3 class="project-title">Blood Donation Management System</h3>
                <p class="project-desc">Full-stack web app built with Spring Boot, Java, MySQL, and jQuery. Implemented JWT authentication with Admin/Donor/Recipient roles and built a responsive UI for managing users, donations, and blood requests.</p>
                <div class="project-tech">
                    <span class="tech-tag">Spring Boot</span>
                    <span class="tech-tag">Java</span>
                    <span class="tech-tag">MySQL</span>
                    <span class="tech-tag">jQuery</span>
                </div>
                <a href="#" class="project-link">View Repository</a>
            </div>
            
            <div class="project-card">
                <div class="project-icon">🌐</div>
                <h3 class="project-title">Portfolio Web</h3>
                <p class="project-desc">Personal portfolio website using HTML, CSS, JavaScript. Fully responsive UI with modern design and optimized accessibility.</p>
                <div class="project-tech">
                    <span class="tech-tag">HTML</span>
                    <span class="tech-tag">CSS</span>
                    <span class="tech-tag">JavaScript</span>
                </div>
                <a href="#" class="project-link">View Repository</a>
            </div>
            
            <div class="project-card">
                <div class="project-icon">📱</div>
                <h3 class="project-title">Notezy – Mobile App</h3>
                <p class="project-desc">Cross-platform note-taking app using React Native + Firebase. Secure authentication, CRUD for notes, real-time syncing, tab navigation.</p>
                <div class="project-tech">
                    <span class="tech-tag">React Native</span>
                    <span class="tech-tag">Firebase</span>
                    <span class="tech-tag">JavaScript</span>
                </div>
                <a href="#" class="project-link">View Repository</a>
            </div>
            
            <div class="project-card">
                <div class="project-icon">🏦</div>
                <h3 class="project-title">Online Banking App Testing</h3>
                <p class="project-desc">Manual + automated testing on a demo banking system. Created test cases, executed UI/functional tests, logged defects, automated flows with Selenium, and validated APIs using Postman.</p>
                <div class="project-tech">
                    <span class="tech-tag">Selenium</span>
                    <span class="tech-tag">Postman</span>
                    <span class="tech-tag">QA Testing</span>
                </div>
                <a href="#" class="project-link">View Repository</a>
            </div>
        </div>
        
        <!-- Stats Section -->
        <div class="section-header">
            <h2>GitHub Stats</h2>
        </div>
        
        <div class="stats-container">
            <div class="stat-card">
                <div class="stat-title">Total Contributions</div>
                <div class="stat-value">1.2k+</div>
            </div>
            <div class="stat-card">
                <div class="stat-title">Repositories</div>
                <div class="stat-value">24</div>
            </div>
            <div class="stat-card">
                <div class="stat-title">Followers</div>
                <div class="stat-value">48</div>
            </div>
            <div class="stat-card">
                <div class="stat-title">Stars Earned</div>
                <div class="stat-value">18</div>
            </div>
        </div>
        
        <!-- Highlights Section -->
        <div class="highlights">
            <h3>Highlights & Fun Facts</h3>
            <ul class="highlight-list">
                <li class="highlight-item">
                    <span class="highlight-icon">💡</span>
                    Passionate about improving software quality and user experience
                </li>
                <li class="highlight-item">
                    <span class="highlight-icon">🎯</span>
                    Currently learning API automation using Postman & Selenium
                </li>
                <li class="highlight-item">
                    <span class="highlight-icon">⚡</span>
                    Always exploring new QA tools and testing methodologies
                </li>
                <li class="highlight-item">
                    <span class="highlight-icon">☕</span>
                    Enjoy coding, testing, and solving real-world software problems
                </li>
            </ul>
        </div>
        
        <!-- Footer -->
        <div class="footer">
            <p>Crafted with <span class="heart">💖</span> by Dilsha Perera</p>
            <p class="signature">✨ Quality Assurance Specialist in the Making ✨</p>
        </div>
    </div>

    <script>
        // Add scroll animations
        document.addEventListener('DOMContentLoaded', function() {
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };
            
            const observer = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, observerOptions);
            
            // Observe all sections for animation
            const sections = document.querySelectorAll('.intro, .social-links, .skills-container, .projects-container, .stats-container, .highlights');
            sections.forEach(section => {
                section.style.opacity = 0;
                section.style.transform = 'translateY(20px)';
                section.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(section);
            });
        });
    </script>
</body>
</html>







<!-- <h1 align="center">Hi 👋, I'm Dilsha Perera</h1>
<h3 align="center">Aspiring QA Engineer | Software Testing Enthusiast | Manual & Automation Testing</h3>
<h3 align="center">A passionate Software Engineering Student from Sri Lanka</h3>

<p align="center">
  🌱 I’m currently learning <b>Selenium, Jira</b> <br>
  💼 Looking to contribute to real-world QA projects and gain hands-on experience <br>
  📫 Reach me at: <a href="mailto:dilshaperera1118@gmail.com">dilshaperera1118@gmail.com</a>
</p>

---

## 🔗 Connect with me
<p align="center">
  <a href="https://linkedin.com/in/dilsha-perera" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://facebook.com/dilsha.perera" target="_blank">
    <img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"/>
  </a>
  <a href="https://instagram.com/dilsha.perera" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram"/>
  </a>
</p>

---

## 🛠 Skills & Tools
<p align="center">
  <img src="https://cdn.worldvectorlogo.com/logos/figma-1.svg" alt="Figma" width="40" height="40"/>
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=spring&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=for-the-badge&logo=intellij-idea&logoColor=white" alt="IntelliJ IDEA"/>
  <img src="https://img.shields.io/badge/WebStorm-000000?style=for-the-badge&logo=webstorm&logoColor=white" alt="WebStorm"/>
  <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code"/>
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman"/>
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="MySQL" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="MongoDB" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git" width="40" height="40"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="40" height="40"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="Linux" width="40" height="40"/>
  <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="Arduino" width="40" height="40"/>
  <img src="https://img.shields.io/badge/JMeter-DB0000?style=for-the-badge&logo=apachejmeter&logoColor=white" alt="JMeter"/>
  <img src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white" alt="Jira"/>
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="React Native" width="40" height="40"/>
  <img src="https://img.shields.io/badge/Tomcat-F8DC75?style=for-the-badge&logo=apachetomcat&logoColor=black" alt="Tomcat"/>
  <img src="https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white" alt="Hibernate"/>
</p>


---

## 💼 Projects

• 🩸 **Blood Donation Management System**
  - Full-stack web app built with **Spring Boot, Java, MySQL, and jQuery**
  - Implemented **JWT authentication** with Admin/Donor/Recipient roles
  - Built a **responsive UI** for managing users, donations, and blood requests
  - 🔗 Repo: ![Repo](https://img.shields.io/badge/Repo-BloodDonation-blue?style=for-the-badge&logo=github&logoColor=white)

• 🌐 **Portfolio Web**
  - Personal portfolio website using **HTML, CSS, JavaScript**
  - Fully **responsive UI** with modern design and optimized accessibility
  - 🔗 Repo: ![Repo](https://img.shields.io/badge/Repo-Portfolio-green?style=for-the-badge&logo=github&logoColor=white)

• 📱 **Notezy – Mobile App**
  - Cross-platform note-taking app using **React Native + Firebase**
  - Secure authentication, CRUD for notes, real-time syncing, tab navigation
  - 🔗 Repo: ![Repo](https://img.shields.io/badge/Repo-Notezy-orange?style=for-the-badge&logo=github&logoColor=white)

• 🏦 **Online Banking App Testing – Ongoing QA Project**
  - Manual + automated testing on a demo banking system
  - Created test cases, executed UI/functional tests
  - Logged defects, automated flows with **Selenium**
  - Validated APIs using **Postman**
  - 🔗 Repo: ![Repo](https://img.shields.io/badge/Repo-BankingQA-red?style=for-the-badge&logo=github&logoColor=white)

---

## 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YOURUSERNAME&show_icons=true&theme=radical" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOURUSERNAME&layout=compact&theme=radical" />
</p>

---

## 🌟 Highlights & Fun Facts
- 💡 Passionate about improving software quality and user experience  
- 🎯 Currently learning API automation using Postman & Selenium  
- ⚡ Always exploring new QA tools and testing methodologies  
- ☕ Enjoy coding, testing, and solving real-world software problems

---

✨ Crafted with 💖 by Dilsha Perera -->




























<!-- <h1 align="center">Hi 👋, I'm Dilsha Perera</h1>
<h3 align="center">A passionate Software Engineering Student from Sri Lanka</h3>

- 🌱 I’m currently learning **JAVA,HTML,CSS**

- 📫 How to reach me **dilshaperera1118@gmail.com**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/dilsha perera" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="dilsha perera" height="30" width="40" /></a>
<a href="https://fb.com/dilsha perera" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="dilsha perera" height="30" width="40" /></a>
<a href="https://instagram.com/dilsha perera" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="dilsha perera" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> </p> -->
