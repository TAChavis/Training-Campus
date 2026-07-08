<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inclusive Sovereignty Inc.</title>
    <style>
        /* Modern Reset and CSS Variables */
        :root {
            --primary: #1e3a8a; /* Deep Trust Blue */
            --secondary: #f59e0b; /* Construction Gold/Amber */
            --dark: #1f2937;
            --light: #f9fafb;
            --white: #ffffff;
            --gray: #6b7280;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        /* Header & Navigation */
        header {
            background-color: var(--primary);
            color: var(--white);
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo h1 {
            font-size: 1.5rem;
            font-weight: 700;
            letter-spacing: 0.5px;
        }

        .logo span {
            color: var(--secondary);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 1.5rem;
        }

        nav ul li a {
            color: var(--white);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--secondary);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(30, 58, 138, 0.85), rgba(31, 41, 55, 0.9)), url('path_to_your_image.jpg') no-repeat center center/cover;
            color: var(--white);
            padding: 8rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.25rem;
            margin-bottom: 2rem;
            color: #e5e7eb;
        }

        .btn {
            background-color: var(--secondary);
            color: var(--dark);
            padding: 0.75rem 2rem;
            border: none;
            border-radius: 4px;
            font-weight: 600;
            text-decoration: none;
            cursor: pointer;
            transition: background 0.3s, transform 0.2s;
            display: inline-block;
        }

        .btn:hover {
            background-color: #d97706;
            transform: translateY(-2px);
        }

        /* Main Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        section {
            margin-bottom: 5rem;
        }

        .section-title {
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            position: relative;
            padding-bottom: 0.5rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 4px;
            background-color: var(--secondary);
        }

        /* Mission Section */
        .mission-box {
            background-color: var(--white);
            padding: 2.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border-left: 5px solid var(--secondary);
        }

        .mission-box p {
            font-size: 1.1rem;
            margin-bottom: 1.5rem;
            color: #4b5563;
        }

        .mission-box p:last-child {
            margin-bottom: 0;
            font-weight: 600;
            color: var(--primary);
        }

        /* Gallery Grid (Facebook Images) */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .gallery-item {
            background-color: var(--white);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }

        .gallery-item:hover {
            transform: scale(1.02);
        }

        .gallery-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
            background-color: #e5e7eb; /* Placeholder if image loads slow */
        }

        .gallery-caption {
            padding: 1rem;
            font-size: 0.95rem;
            color: var(--gray);
            text-align: center;
            border-top: 1px solid #f3f4f6;
        }

        /* Leadership & Structure */
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
            gap: 2.5rem;
        }

        .card {
            background-color: var(--white);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .card ul {
            list-style-type: none;
            margin-top: 1rem;
        }

        .card ul li {
            padding: 0.5rem 0;
            border-bottom: 1px solid #f3f4f6;
            display: flex;
            justify-content: space-between;
        }

        .card ul li:last-child {
            border-bottom: none;
        }

        .badge {
            background-color: #eff6ff;
            color: var(--primary);
            padding: 0.25rem 0.75rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 600;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: #9ca3af;
            padding: 3rem 2rem;
            font-size: 0.9rem;
            border-top: 4px solid var(--primary);
        }

        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 2rem;
        }

        .footer-info h3 {
            color: var(--white);
            margin-bottom: 1rem;
        }

        .footer-links ul {
            list-style: none;
        }

        .footer-links ul li {
            margin-bottom: 0.5rem;
        }

        .footer-links ul li a {
            color: #9ca3af;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-links ul li a:hover {
            color: var(--white);
        }

        .footer-bottom {
            max-width: 1200px;
            margin: 2rem auto 0 auto;
            padding-top: 1.5rem;
            border-top: 1px solid #374151;
            text-align: center;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }
            .hero h2 {
                font-size: 2.2rem;
            }
            .grid-2 {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <!-- Header & Navigation -->
    <header>
        <div class="nav-container">
            <div class="logo">
                <h1>INCLUSIVE <span>SOVEREIGNTY</span></h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#about">Our Mission</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#governance">Leadership</a></li>
                    <li><a href="https://www.facebook.com/share/1BXszzsm5F/?mibextid=wwXIfr" target="_blank">Facebook</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h2>Building Pathways to Economic Independence</h2>
            <p>Empowering adults and youth through hands-on skilled trades education, workforce development, and community investment.</p>
            <a href="#about" class="btn">Learn More About Our Campus</a>
        </div>
    </section>

    <!-- Main Content Container -->
    <div class="container">

        <!-- Mission Statement Section -->
        <section id="about">
            <h2 class="section-title">Our Mission & Purpose</h2>
            <div class="mission-box">
                <p>Inclusive Sovereignty Inc. is dedicated to building stronger communities by creating pathways to economic independence through skilled trades education, workforce development, and community investment. Our mission is to acquire and develop land that serves as a hands-on training campus where adults and young people can learn residential and commercial construction from the ground up—from site preparation and infrastructure to the completion of quality homes and facilities.</p>
                <p>Drawing upon decades of professional experience in construction management, project supervision, safety compliance, quality control, and workforce leadership, Inclusive Sovereignty Inc. prepares participants with industry-recognized skills, practical experience, and mentorship that lead to sustainable careers, entrepreneurship, and financial self-sufficiency.</p>
                <p>We believe every individual deserves the opportunity to learn a valuable trade, earn a living wage, and contribute to the revitalization of their community. Through strategic partnerships, responsible land development, and comprehensive workforce training, Inclusive Sovereignty Inc. seeks to reduce barriers to employment, strengthen the skilled labor force, and create lasting economic opportunities for underserved communities.</p>
                <p><strong>Our Vision:</strong> To develop a model training community where education, employment, housing, and community development work together to empower future generations and build a legacy of opportunity, self-reliance, and inclusive prosperity.</p>
            </div>
        </section>

        <!-- Gallery Section for Facebook Images -->
        <section id="gallery">
            <h2 class="section-title">Campus & Program Gallery</h2>
            <p style="color: var(--gray); margin-bottom: 1.5rem;">A glimpse into our community development, training initiatives, and community impact.</p>
            <div class="gallery-grid">
                
                <!-- Image 1 -->
                <div class="gallery-item">
                    <img src="path_to_your_image1.jpg" alt="Inclusive Sovereignty Community Work 1">
                    <div class="gallery-caption">Hands-on Training & Infrastructure Development</div>
                </div>

                <!-- Image 2 -->
                <div class="gallery-item">
                    <img src="path_to_your_image2.jpg" alt="Inclusive Sovereignty Community Work 2">
                    <div class="gallery-caption">Building Stronger Foundations for Our Future</div>
                </div>

                <!-- Image 3 -->
                <div class="gallery-item">
                    <img src="path_to_your_image3.jpg" alt="Inclusive Sovereignty Community Work 3">
                    <div class="gallery-caption">Workforce Leadership & Sustainable Careers</div>
                </div>

            </div>
            <div style="text-align: center; margin-top: 2rem;">
                <a href="https://www.facebook.com/share/1BXszzsm5F/?mibextid=wwXIfr" target="_blank" class="btn" style="background-color: transparent; border: 2px solid var(--primary); color: var(--primary);">View Full Gallery on Facebook</a>
            </div>
        </section>

        <!-- Governance & Organizational Details -->
        <section id="governance">
            <h2 class="section-title">Organizational Structure</h2>
            <div class="grid-2">
                
                <!-- Board of Directors -->
                <div class="card">
                    <h3>Leadership & Board</h3>
                    <p style="color: var(--gray); font-size: 0.9rem; margin-bottom: 1rem;">The dedicated individuals steering our mission forward.</p>
                    <ul>
                        <li><span>Todd A. Chavis II</span> <span class="badge">President & Director</span></li>
                        <li><span>Lakeya R. Chavis</span> <span class="badge">Secretary</span></li>
                        <li><span>Anthony Moultrie</span> <span class="badge">Director</span></li>
                        <li><span>Tywillie Chavis</span> <span class="badge">Director</span></li>
                    </ul>
                </div>

                <!-- Entity Information -->
                <div class="card">
                    <h3>Corporate Foundation</h3>
                    <p style="color: var(--gray); font-size: 0.9rem; margin-bottom: 1rem;">Legally organized exclusively for public benefit and charitable purposes.</p>
                    <ul>
                        <li><span>Entity Type</span> <strong>Public Benefit Corporation</strong></li>
                        <li><span>State of Incorporation</span> <strong>South Carolina</strong></li>
                        <li><span>IRS Status Filed</span> <strong>501(c)(3) Charitable Purpose</strong></li>
                        <li><span>Focus Areas</span> <strong>Trades Education & Workforce Development</strong></li>
                    </ul>
                </div>

            </div>
        </section>

    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-container">
            <div class="footer-info">
                <h3>Inclusive Sovereignty Inc.</h3>
                <p>Principal Office:<br>513 Azalee Grands Pl<br>Moncks Corner, South Carolina 29461</p>
            </div>
            <div class="footer-links">
                <h3>Quick Links</h3>
                <ul>
                    <li><a href="#about">Our Mission</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#governance">Our Structure</a></li>
                    <li><a href="https://www.facebook.com/share/1BXszzsm5F/?mibextid=wwXIfr" target="_blank">Follow Us on Facebook</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2026 Inclusive Sovereignty Inc. Organized and operated exclusively for charitable and educational purposes under Section 501(c)(3).</p>
        </div>
    </footer>

</body>
</html>
