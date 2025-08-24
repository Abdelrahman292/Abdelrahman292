<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abdelrahman Tahir - Data Analyst</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --card-shadow: 0 10px 20px rgba(0, 0, 0, 0.12);
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: var(--text-color);
            line-height: 1.6;
            padding: 2rem;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        }
        
        header {
            background: linear-gradient(120deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 3rem 2rem;
            text-align: center;
            position: relative;
        }
        
        .profile {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 1.5rem;
        }
        
        .profile-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid rgba(255, 255, 255, 0.3);
            box-shadow: var(--card-shadow);
        }
        
        .profile-content h1 {
            font-size: 2.8rem;
            margin-bottom: 0.5rem;
        }
        
        .profile-content h2 {
            font-size: 1.5rem;
            font-weight: 400;
            opacity: 0.9;
            margin-bottom: 1rem;
        }
        
        .tagline {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            border-radius: 50%;
            font-size: 1.3rem;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background: white;
            color: var(--secondary-color);
            transform: translateY(-5px);
        }
        
        main {
            padding: 3rem 2rem;
        }
        
        .section {
            margin-bottom: 3rem;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 2.5rem;
            color: var(--primary-color);
            position: relative;
            padding-bottom: 15px;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, var(--secondary-color), var(--accent-color));
            border-radius: 2px;
        }
        
        .about-content {
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.1rem;
        }
        
        .certification {
            text-align: center;
            margin-top: 2rem;
            padding: 1.5rem;
            background: var(--light-color);
            border-radius: 10px;
            max-width: 600px;
            margin: 2rem auto;
            box-shadow: var(--card-shadow);
        }
        
        .tools-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        
        .tool-category {
            background: white;
            border-radius: 10px;
            padding: 1.5rem;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
            border-top: 4px solid var(--secondary-color);
        }
        
        .tool-category:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .tool-category h3 {
            color: var(--primary-color);
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .tool-category h3 i {
            color: var(--secondary-color);
        }
        
        .tools-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
        }
        
        .tool {
            background: var(--light-color);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        .tool i {
            color: var(--secondary-color);
        }
        
        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 3rem;
        }
        
        .stat-card {
            background: white;
            border-radius: 10px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
        }
        
        .stat-card:hover h3 {
            color: white;
        }
        
        .stat-card h3 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
            color: var(--secondary-color);
        }
        
        .projects-showcase {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .project-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        .project-content h3 {
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }
        
        .project-content p {
            margin-bottom: 1rem;
            color: #666;
        }
        
        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
        }
        
        .project-tag {
            background: var(--light-color);
            padding: 5px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
        }
        
        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: var(--secondary-color);
            color: white;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            margin-top: 1rem;
        }
        
        .btn:hover {
            background: var(--primary-color);
            transform: translateY(-3px);
        }
        
        footer {
            background: var(--dark-color);
            color: white;
            text-align: center;
            padding: 2.5rem 2rem;
        }
        
        .contact-info {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .contact-info p {
            margin: 1rem 0;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .copyright {
            margin-top: 2rem;
            opacity: 0.8;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            body {
                padding: 1rem;
            }
            
            .profile-content h1 {
                font-size: 2.2rem;
            }
            
            .profile-content h2 {
                font-size: 1.3rem;
            }
            
            .tools-container {
                grid-template-columns: 1fr;
            }
            
            .stats {
                grid-template-columns: 1fr;
            }
        }
        
        /* Animation */
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .animated {
            animation: fadeIn 1s ease-out forwards;
        }
        
        .delay-1 {
            animation-delay: 0.2s;
        }
        
        .delay-2 {
            animation-delay: 0.4s;
        }
        
        .delay-3 {
            animation-delay: 0.6s;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="profile">
                <!-- Replace with your actual image -->
                <img src="https://placehold.co/180x180/3498db/FFFFFF?text=AT" alt="Abdelrahman Tahir" class="profile-img">
                <div class="profile-content">
                    <h1>Abdelrahman Tahir</h1>
                    <h2>Data Analyst & Visualization Specialist</h2>
                    <p class="tagline">Transforming raw data into actionable insights and compelling visual stories</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-github"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-medium-m"></i></a>
                    </div>
                </div>
            </div>
        </header>
        
        <main>
            <section class="section animated">
                <h2 class="section-title">About Me</h2>
                <div class="about-content">
                    <p>I am a passionate data analyst with expertise in transforming complex datasets into meaningful insights through advanced analytics and compelling data visualizations. My goal is to help organizations make data-driven decisions by telling stories with data.</p>
                    
                    <div class="certification">
                        <h3><i class="fas fa-certificate"></i> Professional Certification</h3>
                        <p>Data Analysis Diploma from DATA ECHO on Udemy</p>
                    </div>
                </div>
            </section>
            
            <section class="section animated delay-1">
                <h2 class="section-title">Technical Skills</h2>
                <div class="tools-container">
                    <div class="tool-category">
                        <h3><i class="fas fa-code"></i> Programming</h3>
                        <div class="tools-list">
                            <span class="tool"><i class="fab fa-python"></i> Python</span>
                            <span class="tool"><i class="fas fa-database"></i> SQL</span>
                            <span class="tool"><i class="fab fa-r-project"></i> R</span>
                        </div>
                    </div>
                    
                    <div class="tool-category">
                        <h3><i class="fas fa-chart-bar"></i> Visualization</h3>
                        <div class="tools-list">
                            <span class="tool"><i class="fas fa-chart-pie"></i> Power BI</span>
                            <span class="tool"><i class="fas fa-chart-line"></i> Tableau</span>
                            <span class="tool"><i class="fas fa-chart-bar"></i> Looker Studio</span>
                        </div>
                    </div>
                    
                    <div class="tool-category">
                        <h3><i class="fas fa-table"></i> Data Processing</h3>
                        <div class="tools-list">
                            <span class="tool"><i class="fas fa-file-excel"></i> Excel</span>
                            <span class="tool"><i class="fas fa-cogs"></i> Alteryx</span>
                            <span class="tool"><i class="fas fa-project-diagram"></i> KNIME</span>
                            <span class="tool"><i class="fas fa-calculator"></i> SPSS</span>
                        </div>
                    </div>
                    
                    <div class="tool-category">
                        <h3><i class="fas fa-brain"></i> Data Science</h3>
                        <div class="tools-list">
                            <span class="tool"><i class="fas fa-code"></i> Pandas</span>
                            <span class="tool"><i class="fas fa-calculator"></i> NumPy</span>
                            <span class="tool"><i class="fas fa-chart-line"></i> Data Storytelling</span>
                        </div>
                    </div>
                </div>
                
                <div class="stats">
                    <div class="stat-card">
                        <h3>15+</h3>
                        <p>Projects Completed</p>
                    </div>
                    <div class="stat-card">
                        <h3>5+</h3>
                        <p>Years Experience</p>
                    </div>
                    <div class="stat-card">
                        <h3>12+</h3>
                        <p>Tools Mastered</p>
                    </div>
                    <div class="stat-card">
                        <h3>10+</h3>
                        <p>Happy Clients</p>
                    </div>
                </div>
            </section>
            
            <section class="section animated delay-2">
                <h2 class="section-title">Featured Projects</h2>
                <div class="projects-showcase">
                    <div class="project-card">
                        <img src="https://placehold.co/600x400/3498db/FFFFFF?text=Sales+Analysis" alt="Sales Dashboard" class="project-img">
                        <div class="project-content">
                            <h3>Sales Performance Dashboard</h3>
                            <p>Interactive dashboard analyzing sales trends and performance metrics across multiple regions.</p>
                            <div class="project-tags">
                                <span class="project-tag">Power BI</span>
                                <span class="project-tag">SQL</span>
                                <span class="project-tag">Data Modeling</span>
                            </div>
                            <a href="#" class="btn">View Project</a>
                        </div>
                    </div>
                    
                    <div class="project-card">
                        <img src="https://placehold.co/600x400/e74c3c/FFFFFF?text=Customer+Segmentation" alt="Customer Segmentation" class="project-img">
                        <div class="project-content">
                            <h3>Customer Segmentation Analysis</h3>
                            <p>Cluster analysis to identify distinct customer segments for targeted marketing strategies.</p>
                            <div class="project-tags">
                                <span class="project-tag">Python</span>
                                <span class="project-tag">K-Means</span>
                                <span class="project-tag">Pandas</span>
                            </div>
                            <a href="#" class="btn">View Project</a>
                        </div>
                    </div>
                    
                    <div class="project-card">
                        <img src="https://placehold.co/600x400/2c3e50/FFFFFF?text=Data+Storytelling" alt="Data Storytelling" class="project-img">
                        <div class="project-content">
                            <h3>Data Storytelling Workshop</h3>
                            <p>Educational materials and examples for effective data communication and visualization.</p>
                            <div class="project-tags">
                                <span class="project-tag">Tableau</span>
                                <span class="project-tag">Storytelling</span>
                                <span class="project-tag">Visualization</span>
                            </div>
                            <a href="#" class="btn">View Project</a>
                        </div>
                    </div>
                </div>
            </section>
        </main>
        
        <footer>
            <h2 class="section-title" style="color: white;">Get In Touch</h2>
            <div class="contact-info">
                <p><i class="fas fa-envelope"></i> Email: your.email@example.com</p>
                <p><i class="fas fa-map-marker-alt"></i> Location: Cairo, Egypt</p>
                <p><i class="fas fa-link"></i> Portfolio: abdelrahman-tahir.github.io</p>
            </div>
            <div class="social-links">
                <a href="#"><i class="fab fa-linkedin-in"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-medium-m"></i></a>
            </div>
            <p class="copyright">© 2023 Abdelrahman Tahir. All Rights Reserved.</p>
        </footer>
    </div>

    <script>
        // Add animation class to elements when they come into view
        document.addEventListener('DOMContentLoaded', function() {
            const animatedElements = document.querySelectorAll('.animated');
            
            animatedElements.forEach(element => {
                element.style.opacity = '0';
            });
            
            setTimeout(() => {
                animatedElements.forEach(element => {
                    element.style.opacity = '1';
                });
            }, 100);
        });
    </script>
</body>
</html>
