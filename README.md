<html lang="en-US">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">

<!-- Begin Jekyll SEO tag v2.8.0 -->
<meta name="generator" content="Jekyll v3.10.0" />
<meta property="og:title" content="website" />
<meta property="og:locale" content="en_US" />
<link rel="canonical" href="https://dioram8.github.io/website/" />
<meta property="og:url" content="https://dioram8.github.io/website/" />
<meta property="og:site_name" content="website" />
<meta property="og:type" content="website" />
<meta name="twitter:card" content="summary" />
<meta property="twitter:title" content="website" />
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"WebSite","headline":"website","name":"website","url":"https://dioram8.github.io/website/"}</script>
<!-- End Jekyll SEO tag -->

    <link rel="stylesheet" href="/website/assets/css/style.css?v=36cb51a06640e0903773793c3b20792f64362ef8">
    <!-- start custom head snippets, customize with your own _includes/head-custom.html file -->

<!-- Setup Google Analytics -->



<!-- You can set your favicon here -->
<!-- link rel="shortcut icon" type="image/x-icon" href="/website/favicon.ico" -->

<!-- end custom head snippets -->

  </head>
  <body>
    <div class="container-lg px-3 my-5 markdown-body">
      
      <h1><a href="https://dioram8.github.io/website/">website</a></h1>
      

      <html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Diyora's Assignment Portal</title>
    <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700&amp;display=swap" rel="stylesheet" />
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600&amp;display=swap" rel="stylesheet" />
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        :root {
            --primary: #a770ff;
            --primary-hover: #cf8fff;
            --bg-dark: #0f0f1e;
            --text-light: rgba(255, 255, 255, 0.8);
            --text-mid: rgba(255, 255, 255, 0.6);
            --card-bg: rgba(15, 15, 30, 0.5);
        }
        
        body {
            background: var(--bg-dark);
            background-image: 
                radial-gradient(circle at 20% 30%, rgba(76, 0, 255, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 70%, rgba(255, 0, 128, 0.15) 0%, transparent 50%);
            color: white;
            text-align: center;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            overflow-x: hidden;
            position: relative;
        }

        /* Animated background */
        .animated-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: -2;
            overflow: hidden;
        }

        .animated-bg .bubble {
            position: absolute;
            border-radius: 50%;
            opacity: 0.1;
            filter: blur(20px);
            animation: float 15s infinite linear;
        }

        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); }
            25% { transform: translateY(-50px) rotate(90deg); }
            50% { transform: translateY(0) rotate(180deg); }
            75% { transform: translateY(50px) rotate(270deg); }
            100% { transform: translateY(0) rotate(360deg); }
        }
        
        .navbar {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 25px;
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(12px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            position: relative;
            z-index: 10;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .navbar h1 {
            font-family: 'Syne', sans-serif;
            font-size: 28px;
            letter-spacing: 2px;
            font-weight: 600;
            text-transform: uppercase;
            background: linear-gradient(90deg, #f0f0f0, var(--primary));
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            position: relative;
        }

        .navbar h1:after {
            content: "";
            position: absolute;
            bottom: -5px;
            left: 25%;
            width: 50%;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--primary), transparent);
        }
        
        .container {
            max-width: 1100px;
            margin: 60px auto;
            display: flex;
            flex-direction: column;
            gap: 40px;
            padding: 0 30px;
            flex-grow: 1;
            position: relative;
        }
        
        .card {
            background: var(--card-bg);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.25);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: 1px solid rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            position: relative;
        }
        
        .card::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, #ff00cc, #3333ff, #00ffff, #ff00cc);
            z-index: -1;
            border-radius: 21px;
            background-size: 400%;
            opacity: 0;
            transition: opacity 0.4s ease;
        }
        
        .card:hover {
            transform: translateY(-10px);
        }
        
        .card:hover::before {
            opacity: 0.5;
            animation: glowingBorder 8s linear infinite;
        }
        
        @keyframes glowingBorder {
            0% { background-position: 0 0; }
            50% { background-position: 400% 0; }
            100% { background-position: 0 0; }
        }
        
        .card-header {
            background: rgba(0, 0, 0, 0.2);
            color: white;
            padding: 25px 30px;
            font-size: 22px;
            font-weight: 700;
            letter-spacing: 1px;
            position: relative;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: 'Syne', sans-serif;
        }
        
        .card-header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
        }
        
        .card-body {
            padding: 35px;
            color: var(--text-light);
        }
        
        /* Assignment Section Styles */
        .assignment-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 30px;
            margin-top: 25px;
        }
        
        .assignment-item {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 16px;
            padding: 15px;
            transition: all 0.5s cubic-bezier(0.19, 1, 0.22, 1);
            position: relative;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 120px;
            border: 1px solid rgba(255, 255, 255, 0.02);
            box-shadow: 0 7px 20px rgba(0, 0, 0, 0.1);
        }
        
        .assignment-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 0;
            background: linear-gradient(to bottom, #ff00cc, #3333ff);
            transition: height 0.5s ease;
        }
        
        .assignment-item:hover {
            background: rgba(255, 255, 255, 0.05);
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .assignment-item:hover::before {
            height: 100%;
        }
        
        .assignment-link {
            color: var(--primary);
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
            position: relative;
            transition: all 0.3s ease;
            padding-bottom: 3px;
            letter-spacing: 0.5px;
            background: linear-gradient(90deg, #fff, var(--primary));
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100%;
            font-family: 'Syne', sans-serif;
        }

        .assignment-link .assignment-date {
            font-size: 12px;
            margin-top: 8px;
            opacity: 0.7;
            font-weight: normal;
        }
        
        .assignment-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            background: linear-gradient(90deg, var(--primary), var(--primary-hover));
            transition: width 0.3s ease;
        }
        
        .assignment-link:hover {
            text-shadow: 0 0 8px rgba(167, 112, 255, 0.5);
        }
        
        .assignment-link:hover::after,
        .assignment-link.uploaded::after {
            width: 80%;
        }
        
        .assignment-item.active {
            border-color: rgba(167, 112, 255, 0.5);
            background: rgba(167, 112, 255, 0.1);
        }
        
        .assignment-item.active::before {
            height: 100%;
        }
        
        footer {
            background: rgba(0, 0, 0, 0.3);
            padding: 25px;
            text-align: center;
            margin-top: auto;
            font-size: 14px;
            letter-spacing: 1px;
            color: var(--text-mid);
            backdrop-filter: blur(10px);
            border-top: 1px solid rgba(255, 255, 255, 0.03);
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 10px;
        }

        .social-links a {
            color: var(--text-mid);
            font-size: 20px;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            color: var(--primary);
            transform: translateY(-3px);
        }
        
        /* Profile Section */
        .profile-section {
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }

        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--primary);
            padding: 5px;
            background: rgba(255, 255, 255, 0.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .profile-info {
            text-align: center;
        }

        .profile-info h2 {
            color: white;
            font-size: 24px;
            margin-bottom: 10px;
            font-family: 'Syne', sans-serif;
        }

        .profile-info p {
            color: var(--text-mid);
            font-size: 16px;
            max-width: 600px;
            margin: 0 auto;
            line-height: 1.6;
        }

        .profile-stats {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
        }

        .stat {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .stat-value {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary);
            font-family: 'Syne', sans-serif;
        }

        .stat-label {
            font-size: 14px;
            color: var(--text-mid);
        }

        /* Progress bar */
        .progress-container {
            width: 100%;
            max-width: 600px;
            margin: 20px auto;
        }

        .progress-label {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
        }

        .progress-track {
            width: 100%;
            height: 8px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            overflow: hidden;
        }

        .progress-bar {
            height: 100%;
            background: linear-gradient(90deg, var(--primary), var(--primary-hover));
            border-radius: 10px;
            width: 50%;
            transition: width 1.5s ease;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            .profile-stats {
                flex-direction: column;
                gap: 15px;
            }
            
            .stat {
                flex-direction: row;
                gap: 10px;
                width: 100%;
                justify-content: center;
            }
            
            .card-body {
                padding: 20px;
            }
        }

        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.05);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 10px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-hover);
        }
    </style>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Create animated background bubbles
            const animatedBg = document.querySelector('.animated-bg');
            const colors = ['#a770ff', '#ff00cc', '#3333ff', '#00ffff'];
            
            for (let i = 0; i < 20; i++) {
                const bubble = document.createElement('div');
                bubble.classList.add('bubble');
                
                const size = Math.random() * 200 + 50;
                const color = colors[Math.floor(Math.random() * colors.length)];
                
                bubble.style.width = `${size}px`;
                bubble.style.height = `${size}px`;
                bubble.style.left = `${Math.random() * 100}%`;
                bubble.style.top = `${Math.random() * 100}%`;
                bubble.style.backgroundColor = color;
                bubble.style.animationDelay = `${Math.random() * 15}s`;
                bubble.style.animationDuration = `${15 + Math.random() * 10}s`;
                
                animatedBg.appendChild(bubble);
            }

            // Animate progress bar on load
            setTimeout(() => {
                document.querySelector('.progress-bar').style.width = '25%';
            }, 500);
            
            // Update stats to reflect new number of assignments
            document.querySelector('.stat-value').textContent = '12';
        });
    </script>
</head>
<body>
    <div class="animated-bg"></div>
    
    <div class="navbar">
        <h1>Diyora's Assignment Portal</h1>
    </div>
    
    <div class="container">
        <!-- Profile Section -->
        <div class="card">
            <div class="card-header">Student Profile</div>
            <div class="card-body">
                <div class="profile-section">
                        <div class="profile-info">
                        <h2>Diyora - Student No: 2417494</h2>
                        <p>IBM student at Dong-A University. Passionate about web development and creative coding.</p>
                        
                        <div class="profile-stats">
                            <div class="stat">
                                <div class="stat-value">12</div>
                                <div class="stat-label">Assignments</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">3</div>
                                <div class="stat-label">Completed</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">9</div>
                                <div class="stat-label">Upcoming</div>
                            </div>
                        </div>

                        <div class="progress-container">
                            <div class="progress-label">
                                <span>Course Progress</span>
                                <span>25%</span>
                            </div>
                            <div class="progress-track">
                                <div class="progress-bar"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Assignment Collection Section -->
        <div class="card">
            <div class="card-header">Assignment Collection</div>
            <div class="card-body">
                <p>Track your assignment progress throughout the semester</p>
                
                <div class="assignment-list">
                    <div class="assignment-item active">
                        <a href="https://docs.google.com/document/d/1z1v-lLQ0GKyZsSDASf-bf2dJ2qaiNxGvPdjN58VEEm0/edit?usp=drive_link" class="assignment-link uploaded">
                            Assignment 1
                            <span class="assignment-date">Due: Feb 15, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item active">
                        <a href="https://dioram8.github.io/assignment2/" class="assignment-link uploaded">
                            Assignment 2
                            <span class="assignment-date">Due: Mar 1, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item active">
                        <a href="https://dioram8.github.io/assignment3/" class="assignment-link uploaded">
                            Assignment 3
                            <span class="assignment-date">Due: Mar 15, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item active">
                        <a href="https://drive.google.com/drive/folders/1NiWr6MC1IktlPcXPBEHMnrXVkMK0a1eC?usp=drive_link" class="assignment-link uploaded">
                            Assignment 4
                            <span class="assignment-date">Due: Apr 1, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 5
                            <span class="assignment-date">Due: Apr 15, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 6
                            <span class="assignment-date">Due: May 1, 2025</span>
                        </a>
                    </div>
                    
                    <!-- Added 6 more assignment buttons -->
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 7
                            <span class="assignment-date">Due: May 15, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 8
                            <span class="assignment-date">Due: Jun 1, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 9
                            <span class="assignment-date">Due: Jun 15, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 10
                            <span class="assignment-date">Due: Jul 1, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 11
                            <span class="assignment-date">Due: Jul 15, 2025</span>
                        </a>
                    </div>
                    
                    <div class="assignment-item">
                        <a href="#" class="assignment-link">
                            Assignment 12
                            <span class="assignment-date">Due: Aug 1, 2025</span>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <footer>
        <div>
            &copy; 2025 Diyora | Dong-A University
        </div>
        <div class="social-links">
            <a href="#" title="GitHub">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="https://github.com/DioraM8" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
                </svg>
            </a>
            <a href="#" title="Email">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="diyoramuslimova7@gmail.com" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
                    <polyline points="22,6 12,13 2,6"></polyline>
                </svg>
            </a>
        </div>
    </footer>
</body>
</html>


      
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
    <script>anchors.add();</script>
  </body>
</html>
