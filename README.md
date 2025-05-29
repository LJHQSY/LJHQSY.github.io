# LJHQSY.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MegaMinds Smart Manufacturing | AI-Driven Solutions for Malaysian SMEs</title>
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
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            background: linear-gradient(45deg, #fff, #a8e6cf);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s ease;
            font-weight: 500;
        }

        .nav-links a:hover {
            color: #a8e6cf;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 120px 0 80px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="50" cy="50" r="1" fill="%23ffffff" opacity="0.1"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
            opacity: 0.3;
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            animation: slideInUp 1s ease-out;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
            animation: slideInUp 1s ease-out 0.2s both;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(45deg, #ff6b6b, #ee5a52);
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            animation: slideInUp 1s ease-out 0.4s both;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(255, 107, 107, 0.4);
        }

        /* Sections */
        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #2c3e50;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(45deg, #667eea, #764ba2);
            border-radius: 2px;
        }

        /* About Section */
        .about {
            background: #f8f9fa;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .about-text h3 {
            color: #2c3e50;
            margin-bottom: 1rem;
            font-size: 1.8rem;
        }

        .about-text p {
            margin-bottom: 1.5rem;
            color: #666;
            font-size: 1.1rem;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
            margin-top: 2rem;
        }

        .stat {
            text-align: center;
            padding: 2rem;
            background: white;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .stat:hover {
            transform: translateY(-5px);
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: bold;
            color: #667eea;
            margin-bottom: 0.5rem;
        }

        /* Solution Section */
        .solution {
            background: white;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2.5rem;
            border-radius: 20px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(102, 126, 234, 0.3);
        }

        .feature-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .feature h3 {
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }

        /* Technology Section */
        .technology {
            background: #f8f9fa;
        }

        .tech-stack {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .tech-item {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s ease;
        }

        .tech-item:hover {
            transform: translateY(-5px);
        }

        .tech-item h4 {
            color: #2c3e50;
            margin-bottom: 1rem;
        }

        /* ROI Section */
        .roi {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .roi-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .roi-chart {
            background: rgba(255,255,255,0.1);
            padding: 2rem;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .roi-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 1rem;
            padding: 1rem;
            background: rgba(255,255,255,0.1);
            border-radius: 10px;
        }

        /* Timeline Section */
        .timeline {
            background: white;
        }

        .timeline-container {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline-item {
            padding: 2rem;
            background: #f8f9fa;
            margin: 2rem 0;
            border-radius: 15px;
            border-left: 5px solid #667eea;
            transition: transform 0.3s ease;
        }

        .timeline-item:hover {
            transform: translateX(10px);
        }

        .timeline-item h4 {
            color: #2c3e50;
            margin-bottom: 1rem;
        }

        /* Contact Section */
        .contact {
            background: #2c3e50;
            color: white;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: 2rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 1rem;
            border: none;
            border-radius: 10px;
            font-size: 1rem;
            background: rgba(255,255,255,0.1);
            color: white;
            backdrop-filter: blur(10px);
        }

        .form-group input::placeholder,
        .form-group textarea::placeholder {
            color: rgba(255,255,255,0.7);
        }

        .submit-btn {
            background: linear-gradient(45deg, #ff6b6b, #ee5a52);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s ease;
            width: 100%;
        }

        .submit-btn:hover {
            transform: translateY(-3px);
        }

        /* Footer */
        footer {
            background: #1a1a1a;
            color: white;
            text-align: center;
            padding: 2rem 0;
        }

        /* Animations */
        @keyframes slideInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .about-grid,
            .roi-grid {
                grid-template-columns: 1fr;
                gap: 2rem;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <div class="logo">MegaMinds</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#solution">Solution</a></li>
                <li><a href="#technology">Technology</a></li>
                <li><a href="#roi">ROI</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>MegaMinds Smart Manufacturing</h1>
                <p>AI-Driven Cross-Departmental Collaborative Solutions for Malaysian SMEs</p>
                <a href="#solution" class="cta-button">Discover Our Solution</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">Bridging the Digital Divide</h2>
            <div class="about-grid">
                <div class="about-text fade-in">
                    <h3>Our Mission</h3>
                    <p>To provide AI-driven cross-departmental collaborative solutions for Malaysia's manufacturing industry, focusing on digital transformation for small and medium-sized enterprises.</p>
                    <p>We recognized that while MNCs have resources for advanced digitalization, 98.5% of Malaysian businesses classified as SMEs remain largely excluded from the Industry 4.0 revolution.</p>
                    <p>Malaysia's manufacturing sector contributes 23% to GDP, yet many component suppliers still operate with processes unchanged since the 1990s.</p>
                </div>
                <div class="stats fade-in">
                    <div class="stat">
                        <div class="stat-number">83%</div>
                        <div>Efficiency Improvement</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">15%</div>
                        <div>Rework Reduction</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">50M</div>
                        <div>Industry Savings (MYR)</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Solution Section -->
    <section id="solution" class="solution">
        <div class="container">
            <h2 class="section-title">Automotive Component Design Change Management System</h2>
            <div class="features-grid">
                <div class="feature fade-in">
                    <div class="feature-icon">🧠</div>
                    <h3>Cultural Intelligence Engine</h3>
                    <p>Trilingual processing (English/Bahasa Malaysia/Mandarin) with natural code-switching support for Malaysian manufacturing environments.</p>
                </div>
                <div class="feature fade-in">
                    <div class="feature-icon">⚡</div>
                    <h3>Lightning Fast Changes</h3>
                    <p>Reduce design change cycles from 48 hours to 8 hours while maintaining quality standards and compliance requirements.</p>
                </div>
                <div class="feature fade-in">
                    <div class="feature-icon">🔍</div>
                    <h3>Intelligent Impact Analysis</h3>
                    <p>AI-powered risk assessment with knowledge graphs mapping part relationships, supplier dependencies, and cultural considerations.</p>
                </div>
                <div class="feature fade-in">
                    <div class="feature-icon">🤝</div>
                    <h3>Relationship-Aware Workflows</h3>
                    <p>Respects Malaysian business culture with hierarchy-aware approval routing and consensus-building decision processes.</p>
                </div>
                <div class="feature fade-in">
                    <div class="feature-icon">📱</div>
                    <h3>AR-Assisted Collaboration</h3>
                    <p>Mobile-first AR interface displaying AI-annotated change impacts with confidence indicators and multilingual support.</p>
                </div>
                <div class="feature fade-in">
                    <div class="feature-icon">📊</div>
                    <h3>PMI Framework Integration</h3>
                    <p>Built on internationally recognized project management standards with Malaysian cultural adaptations.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Technology Section -->
    <section id="technology" class="technology">
        <div class="container">
            <h2 class="section-title">Technology Stack</h2>
            <div class="tech-stack">
                <div class="tech-item fade-in">
                    <h4>Natural Language Processing</h4>
                    <p>Fine-tuned GPT-4 for Malaysian manufacturing terminology with 95% accuracy for multilingual documentation</p>
                </div>
                <div class="tech-item fade-in">
                    <h4>Knowledge Graph</h4>
                    <p>Neo4j-based relationship mapping for parts, processes, and stakeholder dependencies</p>
                </div>
                <div class="tech-item fade-in">
                    <h4>Computer Vision</h4>
                    <p>Defect detection and visual change analysis with Malaysian manufacturing image training</p>
                </div>
                <div class="tech-item fade-in">
                    <h4>Cloud Infrastructure</h4>
                    <p>AWS/Azure deployment for scalability with backward compatibility for legacy systems</p>
                </div>
                <div class="tech-item fade-in">
                    <h4>AR Platform</h4>
                    <p>Microsoft HoloLens integration for immersive change visualization and collaboration</p>
                </div>
                <div class="tech-item fade-in">
                    <h4>API Integration</h4>
                    <p>RESTful connections with existing ERP systems including legacy 1990s platforms</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ROI Section -->
    <section id="roi" class="roi">
        <div class="container">
            <h2 class="section-title">Return on Investment</h2>
            <div class="roi-grid">
                <div class="fade-in">
                    <h3>Project Investment: MYR 320,000</h3>
                    <p>Competitive with similar Malaysian SME digitalization projects, with 50% Industry4WRD grant potential.</p>
                    <p><strong>Payback Period:</strong> 12-18 months through efficiency gains and quality improvements.</p>
                    <p><strong>Individual SME Savings:</strong> MYR 80,000-150,000 annually through reduced rework and faster cycles.</p>
                </div>
                <div class="roi-chart fade-in">
                    <h4>Cost Breakdown</h4>
                    <div class="roi-item">
                        <span>Development Costs</span>
                        <span>MYR 150,000 (46.9%)</span>
                    </div>
                    <div class="roi-item">
                        <span>Infrastructure & Equipment</span>
                        <span>MYR 80,000 (25.0%)</span>
                    </div>
                    <div class="roi-item">
                        <span>Training & Implementation</span>
                        <span>MYR 40,000 (12.5%)</span>
                    </div>
                    <div class="roi-item">
                        <span>Contingency & Operations</span>
                        <span>MYR 50,000 (15.6%)</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Timeline Section -->
    <section class="timeline">
        <div class="container">
            <h2 class="section-title">Implementation Timeline</h2>
            <div class="timeline-container">
                <div class="timeline-item fade-in">
                    <h4>Phase 1: Initiating & Planning (Weeks 1-8)</h4>
                    <p>Project charter development, stakeholder analysis, risk assessment, and technical specifications with cultural sensitivity training.</p>
                </div>
                <div class="timeline-item fade-in">
                    <h4>Phase 2: Technical Development (Weeks 9-20)</h4>
                    <p>NLP system prototype, knowledge graph framework, AR interface mockup with mixed-language processing capability.</p>
                </div>
                <div class="timeline-item fade-in">
                    <h4>Phase 3: Testing & Validation (Weeks 21-28)</h4>
                    <p>User acceptance testing, performance validation, cultural adaptation verification with multi-ethnic workforce testing.</p>
                </div>
                <div class="timeline-item fade-in">
                    <h4>Phase 4: Deployment & Closing (Weeks 29-36)</h4>
                    <p>Full system deployment, training completion, supplier relationship integration, and PDPA compliance certification.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Partner With Us</h2>
            <form class="contact-form">
                <div class="form-group">
                    <label for="company">Company Name</label>
                    <input type="text" id="company" placeholder="Your Company Name" required>
                </div>
                <div class="form-group">
                    <label for="name">Contact Person</label>
                    <input type="text" id="name" placeholder="Your Name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" placeholder="your.email@company.com" required>
                </div>
                <div class="form-group">
                    <label for="employees">Company Size</label>
                    <input type="text" id="employees" placeholder="Number of employees" required>
                </div>
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" rows="5" placeholder="Tell us about your manufacturing challenges and digital transformation goals..."></textarea>
                </div>
                <button type="submit" class="submit-btn">Request Consultation</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 MegaMinds Smart Manufacturing Sdn. Bhd. | Empowering Malaysian SMEs with AI-Driven Solutions</p>
            <p>🇲🇾 Made in Malaysia for Malaysian Manufacturing Excellence</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Fade in animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Form submission
        document.querySelector('.contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your interest! We will contact you within 24 hours to discuss your digital transformation journey.');
        });

        // Dynamic stats counter
        function animateStats() {
            const stats = document.querySelectorAll('.stat-number');
            stats.forEach(stat => {
                const target = stat.textContent;
                const isPercentage = target.includes('%');
                const isCurrency = target.includes('M');
                let currentValue = 0;
                const increment = target.replace(/[^\d]/g, '') / 50;
                
                const counter = setInterval(() => {
                    currentValue += increment;
                    if (currentValue >= target.replace(/[^\d]/g, '')) {
                        currentValue = target.replace(/[^\d]/g, '');
                        clearInterval(counter);
                    }
                    
                    if (isPercentage) {
                        stat.textContent = Math.floor(currentValue) + '%';
                    } else if (isCurrency) {
                        stat.textContent = Math.floor(currentValue) + 'M';
                    } else {
                        stat.textContent = Math.floor(currentValue);
                    }
                }, 50);
            });
        }

        // Trigger stats animation when section is visible
        const statsObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    animateStats();
                    statsObserver.unobserve(entry.target);
                }
            });
        });

        const statsSection = document.querySelector('.stats');
        if (statsSection) {
            statsObserver.observe(statsSection);
        }
    </script>
</body>
</html>
