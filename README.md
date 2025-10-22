# Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bhavani Sri Ramya | Strategic Operator & Product Leader</title>
    <style>
        :root {
            --primary: #1a365d;
            --secondary: #2d3748;
            --accent: #d69e2e;
            --light: #f7fafc;
            --gray: #e2e8f0;
            --dark: #2d3748;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--secondary);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Navigation */
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 2rem;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--accent);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 5rem 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: var(--primary);
            padding: 0.8rem 1.5rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
        }
        
        .btn:hover {
            background-color: #ecc94b;
            transform: translateY(-2px);
        }
        
        /* Section Styling */
        section {
            padding: 5rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            color: var(--primary);
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--accent);
            margin: 0.5rem auto;
        }
        
        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 3rem;
            align-items: center;
        }
        
        .profile-img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .skill-category {
            background-color: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .skill-category:hover {
            transform: translateY(-5px);
        }
        
        .skill-category h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            border-bottom: 2px solid var(--accent);
            padding-bottom: 0.5rem;
        }
        
        .skill-list {
            list-style: none;
        }
        
        .skill-list li {
            margin-bottom: 0.5rem;
            padding-left: 1.5rem;
            position: relative;
        }
        
        .skill-list li:before {
            content: '▸';
            position: absolute;
            left: 0;
            color: var(--accent);
        }
        
        /* Experience Section */
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .timeline:before {
            content: '';
            position: absolute;
            left: 50%;
            top: 0;
            bottom: 0;
            width: 2px;
            background-color: var(--gray);
            transform: translateX(-50%);
        }
        
        .timeline-item {
            margin-bottom: 3rem;
            position: relative;
            width: 50%;
            padding-right: 3rem;
        }
        
        .timeline-item:nth-child(even) {
            margin-left: 50%;
            padding-right: 0;
            padding-left: 3rem;
        }
        
        .timeline-content {
            background-color: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            position: relative;
        }
        
        .timeline-content:after {
            content: '';
            position: absolute;
            top: 20px;
            right: -10px;
            width: 0;
            height: 0;
            border-top: 10px solid transparent;
            border-bottom: 10px solid transparent;
            border-left: 10px solid white;
        }
        
        .timeline-item:nth-child(even) .timeline-content:after {
            right: auto;
            left: -10px;
            border-left: none;
            border-right: 10px solid white;
        }
        
        .timeline-date {
            display: inline-block;
            background-color: var(--accent);
            color: var(--primary);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: bold;
            margin-bottom: 1rem;
        }
        
        .timeline-content h3 {
            color: var(--primary);
            margin-bottom: 0.5rem;
        }
        
        .timeline-content h4 {
            color: var(--secondary);
            margin-bottom: 1rem;
            font-weight: normal;
        }
        
        .timeline-content ul {
            list-style: none;
        }
        
        .timeline-content li {
            margin-bottom: 0.5rem;
            padding-left: 1.5rem;
            position: relative;
        }
        
        .timeline-content li:before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--accent);
        }
        
        /* Achievements Section */
        .achievements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .achievement-card {
            background-color: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            text-align: center;
            transition: transform 0.3s;
        }
        
        .achievement-card:hover {
            transform: translateY(-5px);
        }
        
        .achievement-icon {
            font-size: 2.5rem;
            color: var(--accent);
            margin-bottom: 1rem;
        }
        
        /* Publications Section */
        .publications-list {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .publication-item {
            background-color: white;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .publication-item:hover {
            transform: translateY(-3px);
        }
        
        .publication-item h3 {
            color: var(--primary);
            margin-bottom: 0.5rem;
        }
        
        .publication-link {
            color: var(--accent);
            text-decoration: none;
            font-weight: bold;
        }
        
        .publication-link:hover {
            text-decoration: underline;
        }
        
        /* Contact Section */
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .contact-info {
            background-color: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .contact-info h3 {
            color: var(--primary);
            margin-bottom: 1rem;
        }
        
        .contact-info p {
            margin-bottom: 1rem;
        }
        
        .contact-info a {
            color: var(--accent);
            text-decoration: none;
        }
        
        .contact-info a:hover {
            text-decoration: underline;
        }
        
        /* Footer */
        footer {
            background-color: var(--primary);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .timeline:before {
                left: 20px;
            }
            
            .timeline-item {
                width: 100%;
                padding-right: 0;
                padding-left: 3rem;
            }
            
            .timeline-item:nth-child(even) {
                margin-left: 0;
                padding-left: 3rem;
            }
            
            .timeline-content:after {
                display: none;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container nav-container">
            <div class="logo">BSR</div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#achievements">Achievements</a></li>
                <li><a href="#publications">Publications</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Bhavani Sri Ramya M</h1>
            <p>A strategic operator and product leader who leverages extensive experience to drive business growth and operational excellence.</p>
            <a href="#contact" class="btn">Get In Touch</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="about-content">
                <div>
                    <img src="https://via.placeholder.com/300x300?text=Professional+Photo" alt="Bhavani Sri Ramya" class="profile-img">
                </div>
                <div>
                    <p>Strategic operator and product leader with extensive experience driving business growth and operational excellence. Skilled leader and problem-solver with exceptional coordination abilities. Strong communicator known for standardizing business activities.</p>
                    <p>Specializing in the end-to-end development of higher-education content, learning materials, and accredited curricula for universities and corporate training programs.</p>
                    <div style="margin-top: 2rem;">
                        <a href="#contact" class="btn">Contact Me</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" style="background-color: var(--gray);">
        <div class="container">
            <h2 class="section-title">Skills & Expertise</h2>
            <div class="skills-container">
                <div class="skill-category">
                    <h3>Academic Expertise</h3>
                    <ul class="skill-list">
                        <li>Academic Administration</li>
                        <li>Curriculum Development</li>
                        <li>Instructional Design</li>
                        <li>Quality Assurance</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Business Strategy</h3>
                    <ul class="skill-list">
                        <li>Financial & Business Acumen</li>
                        <li>Leadership & Business Strategy</li>
                        <li>Strategic Planning</li>
                        <li>Operational Excellence</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Tools & Technologies</h3>
                    <ul class="skill-list">
                        <li>Canva</li>
                        <li>MS PowerPoint (Advanced)</li>
                        <li>CANYA</li>
                        <li>Financial Modeling</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience">
        <div class="container">
            <h2 class="section-title">Professional Experience</h2>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-content">
                        <span class="timeline-date">Jan 2023 – Present</span>
                        <h3>Academic SME & Freelance Curriculum Developer</h3>
                        <h4>Independent Consultant</h4>
                        <ul>
                            <li>Developed authoritative academic content and learning materials for university and corporate clients</li>
                            <li>Served as quality-assurance SME for Tata Consultancy Services (TCS)</li>
                            <li>Developed structured educational content for Scottish Qualifications Authority (SQA)</li>
                            <li>Authored academic scripts and book chapters for YCMOU & Assam DownTown University</li>
                            <li>Created contemporary curriculum PPTs and case studies for Atlas Skilltech University</li>
                        </ul>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="timeline-content">
                        <span class="timeline-date">Jan 2023 – September 2025</span>
                        <h3>Executive Assistant to Joint Director, Assistant Professor, Academic Coordinator</h3>
                        <h4>Integral Institute of Advanced Management</h4>
                        <ul>
                            <li>Designed academic "products" by integrating curriculum and educational standards</li>
                            <li>Established and formalized Standard Operating Procedures (SOPs)</li>
                            <li>Evaluated and analyzed student learning outcomes and academic performance</li>
                            <li>Directed all operational aspects of Entrepreneurship Cell and Incubation</li>
                            <li>Delivered high-impact lectures in Entrepreneurship, Finance, and Marketing</li>
                        </ul>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="timeline-content">
                        <span class="timeline-date">2018-2022</span>
                        <h3>Operations Analyst</h3>
                        <h4>Telangana Industrial Health Clinic Ltd (Hyderabad)</h4>
                        <ul>
                            <li>Led operational turnaround of struggling enterprises, reviving 25 businesses</li>
                            <li>Designed and framed Standard Operating Procedures (SOPs)</li>
                            <li>Managed project budgets for business revival initiatives</li>
                            <li>Developed and executed strategic marketing campaigns</li>
                            <li>Created detailed financial projections and business models</li>
                        </ul>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="timeline-content">
                        <span class="timeline-date">2013-2014</span>
                        <h3>Financial Analyst</h3>
                        <h4>GENPACT</h4>
                        <ul>
                            <li>Ensured due diligence in audits of critical business processes</li>
                            <li>Monitored accounts with over 100 vendors</li>
                            <li>Conducted cash flow analyses to identify discrepancies</li>
                            <li>Mentored and developed four junior analysts</li>
                            <li>Played pivotal role in closing accounts payable books</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Achievements Section -->
    <section id="achievements" style="background-color: var(--gray);">
        <div class="container">
            <h2 class="section-title">Awards & Achievements</h2>
            <div class="achievements-grid">
                <div class="achievement-card">
                    <div class="achievement-icon">🏆</div>
                    <h3>KALA Research & NCIRD</h3>
                    <p>Young Academician 2025</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">⭐</div>
                    <h3>vIRSD Awards 2024</h3>
                    <p>International Award for Exemplary Academic Leaders 2024</p>
                </div>
                <div class="achievement-card">
                    <div class="achievement-icon">💼</div>
                    <h3>LinkedIn Top Voice</h3>
                    <p>Business Strategy</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Publications Section -->
    <section id="publications">
        <div class="container">
            <h2 class="section-title">Publications</h2>
            <div class="publications-list">
                <div class="publication-item">
                    <h3>Factors Affecting Customers' Lifetime Value of Fintech Services</h3>
                    <p>International Journal of Scientific Research in Engineering & Management (USREM)</p>
                    <a href="https://ijsrem.com/volume08issue08august2024/" class="publication-link" target="_blank">Read Publication</a>
                </div>
                <div class="publication-item">
                    <h3>Financial Management Strategies For Sustainability Of Micro-Small-Enterprises In North Coastal Districts Of Andhra Pradesh</h3>
                    <p>Journal of Business, Management and Economics, Engineering (VILNIUS TECH Journals)</p>
                    <a href="https://businessmanagementeconomic.org/article/view-2024/02-557.html" class="publication-link" target="_blank">Read Publication</a>
                </div>
                <div class="publication-item">
                    <h3>TS-iPass – Study of all Districts and Industry Sectors in Telangana</h3>
                    <p>Telangana Industrial Health Clinic Ltd</p>
                    <a href="https://www.tihcl.telangana.gov.in/pdf/TS-iPASS.pdf" class="publication-link" target="_blank">Read Publication</a>
                </div>
                <div class="publication-item">
                    <h3>Raising Red Flags</h3>
                    <p>Global Linker Telangana</p>
                    <a href="https://ts-msmc.globallinker.com/bizforum/article/look-out-for-these-lsquored-flags-whenyou-start-a-business/31827" class="publication-link" target="_blank">Read Publication</a>
                </div>
                <div class="publication-item">
                    <h3>Silver Lining Budget</h3>
                    <p>Global Linker Telangana</p>
                    <a href="https://ts-msmc.globallinker.com/bizforum/article/a-silver-lining budget/63318/" class="publication-link" target="_blank">Read Publication</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" style="background-color: var(--gray);">
        <div class="container">
            <h2 class="section-title">Get In Touch</h2>
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <p><strong>Phone:</strong> 8555037554</p>
                    <p><strong>Email:</strong> ramya.madhura@gmail.com</p>
                    <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/bhavanisriramya/" target="_blank">bhavanisriramya</a></p>
                </div>
                <div class="contact-info">
                    <h3>Education</h3>
                    <p><strong>MBA – International Finance & Banking</strong><br>GITAM School of International Business</p>
                    <p><strong>PGD – Intellectual Property Rights</strong><br>Andhra University</p>
                </div>
                <div class="contact-info">
                    <h3>Certifications</h3>
                    <p>• UGC NET – MANAGEMENT</p>
                    <p>• IIBF – MSME Certification</p>
                    <p>• IID - Design Thinking</p>
                    <p>• AMDP – Technopreneurship</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 Bhavani Sri Ramya M. All Rights Reserved.</p>
        </div>
    </footer>
</body>
</html>
