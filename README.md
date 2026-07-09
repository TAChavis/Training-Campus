<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inclusive Sovereignty Inc.</title>
    
    <script src="https://www.paypal.com/sdk/js?client-id=BAA_x2uzVfOe-pL9f8EBeHVcE9ZkdLqm7uA77VlbWcVh-kl8x3_Pf9yjTngf2OVRE_Np1kP8SCNnrp8iuw&components=hosted-buttons&enable-funding=venmo&currency=USD"></script>
    
    <style>
        :root {
            --primary: #1e3a8a;
            --secondary: #f59e0b;
            --dark: #1f2937;
            --light: #f3f4f6;
            --white: #ffffff;
            --gray: #6b7280;
            --accent-green: #10b981;
            --card-gradient-1: linear-gradient(135deg, #fdf8ee 0%, #fef3c7 100%);
            --card-gradient-2: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        header {
            background-color: var(--primary);
            color: var(--white);
            padding: 1.5rem;
            text-align: center;
        }
        header h1 {
            font-size: 1.8rem;
        }
        header span {
            color: var(--secondary);
        }
        .hero {
            background: linear-gradient(rgba(15, 23, 42, 0.75), rgba(30, 58, 138, 0.75)), url('https://images.unsplash.com/photo-1504307651254-35680f356dfd?q=80&w=1200&auto=format&fit=crop') no-repeat center center/cover;
            color: var(--white);
            padding: 6rem 1.5rem;
            text-align: center;
        }
        .hero h2 {
            font-size: 2.2rem;
            margin-bottom: 1rem;
        }
        .hero p {
            max-width: 700px;
            margin: 0 auto 2rem auto;
            font-size: 1.1rem;
        }
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 3rem 1.5rem;
        }
        .section-title {
            font-size: 1.8rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            border-bottom: 4px solid var(--secondary);
            padding-bottom: 0.5rem;
            display: inline-block;
        }
        .mission-box {
            background: var(--white);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 10px 15px -3px rgba(0,0,0,0.05);
            margin-bottom: 2rem;
            border-top: 4px solid var(--primary);
        }
        .mission-box p {
            margin-bottom: 1.2rem;
            font-size: 1.05rem;
            color: #4b5563;
        }
        .donation-banner {
            background-color: #eff6ff;
            border-left: 5px solid var(--primary);
            padding: 1.5rem;
            border-radius: 0 8px 8px 0;
            margin-bottom: 3rem;
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 1.5rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        .donation-text h4 {
            color: var(--primary);
            font-size: 1.2rem;
            margin-bottom: 0.25rem;
        }
        .donation-text p {
            color: #4b5563;
            font-size: 0.95rem;
        }
        .paypal-direct-link {
            color: var(--primary);
            font-weight: bold;
            text-decoration: underline;
            font-size: 1.05rem;
            transition: color 0.2s ease;
        }
        .paypal-direct-link:hover {
            color: var(--secondary);
        }
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        .gallery-item {
            background: var(--white);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        .gallery-item:hover {
            transform: translateY(-5px);
        }
        .gallery-item img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }
        .gallery-caption {
            padding: 1rem;
            font-weight: bold;
            color: var(--primary);
            text-align: center;
        }
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        .card {
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        .card-leadership {
            background: var(--card-gradient-1);
            border-left: 6px solid var(--secondary);
        }
        .card-framework {
            background: var(--card-gradient-2);
            border-left: 6px solid var(--primary);
        }
        .card h3 {
            margin-bottom: 1.2rem;
            color: var(--primary);
            font-size: 1.4rem;
        }
        .card ul {
            list-style: none;
            margin-bottom: 1.5rem;
        }
        .card ul li {
            padding: 0.75rem 0;
            border-bottom: 1px solid rgba(0, 0, 0, 0.08);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .card ul li span {
            font-weight: 600;
        }
        .history-section {
            background: var(--white);
            padding: 3rem 2rem;
            border-radius: 12px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            margin-top: 2rem;
            scroll-margin-top: 20px;
        }
        .history-profile {
            margin-bottom: 2.5rem;
            padding-bottom: 2.5rem;
            border-bottom: 1px solid #e5e7eb;
        }
        .history-profile:last-child {
            margin-bottom: 0;
            padding-bottom: 0;
            border-bottom: none;
        }
        .history-profile h3 {
            color: var(--primary);
            font-size: 1.4rem;
            margin-bottom: 0.25rem;
        }
        .history-profile .title {
            color: var(--secondary);
            font-weight: bold;
            margin-bottom: 1rem;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 0.05em;
        }
        p.bio-text {
            color: #4b5563;
            font-size: 1.05rem;
            margin-bottom: 1rem;
        }
        footer {
            background-color: #111827;
            color: #9ca3af;
            padding: 3rem 1.5rem;
            text-align: center;
            margin-top: 4rem;
            font-size: 0.9rem;
        }
        .btn {
            background-color: var(--secondary);
            color: var(--dark);
            padding: 0.75rem 1.5rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            transition: background 0.2s ease, transform 0.2s ease;
            text-align: center;
        }
        .btn:hover {
            background-color: #d97706;
        }
        .btn-sm {
            padding: 0.5rem 1rem;
            font-size: 0.9rem;
            background-color: var(--primary);
            color: var(--white);
            border-radius: 6px;
            align-self: flex-start;
        }
        .btn-sm:hover {
            background-color: #1d4ed8;
        }
    </style>
</head>
<body>

    <header>
        <h1>INCLUSIVE <span>SOVEREIGNTY INC.</span></h1>
    </header>

    <section class="hero">
        <h2>Pathways to Economic Independence</h2>
        <p>Empowering adults and youth through hands-on skilled trades education, workforce development, and community investment.</p>
        <a href="https://www.facebook.com/share/1BXszzsm5F/?mibextid=wwXIfr" target="_blank" class="btn">Visit Our Facebook Page</a>
    </section>

    <div class="container">
        
        <h2 class="section-title">Our Mission</h2>
        <div class="mission-box">
            <p>Inclusive Sovereignty Inc. is dedicated to building stronger communities by creating pathways to economic independence through skilled trades education, workforce development, and community investment. Our mission is to acquire and develop land that serves as a hands-on training campus where adults and young people can learn residential and commercial construction from the ground up—from site preparation and infrastructure to the completion of quality homes and facilities.</p>
            <p>Drawing upon decades of professional experience in construction management, project supervision, safety compliance, quality control, and workforce leadership, Inclusive Sovereignty Inc. prepares participants with industry-recognized skills, practical experience, and mentorship that lead to sustainable careers, entrepreneurship, and financial self-sufficiency.</p>
            <p>We believe every individual deserves the opportunity to learn a valuable trade, earn a living wage, and contribute to the revitalization of their community. Through strategic partnerships, responsible land development, and comprehensive workforce training, Inclusive Sovereignty Inc. seeks to reduce barriers to employment, strengthen the skilled labor force, and create lasting economic opportunities for underserved communities.</p>
            <p><strong>Our Vision:</strong> To develop a model training community where education, employment, housing, and community development work together to empower future generations and build a legacy of opportunity, self-reliance, and inclusive prosperity.</p>
        </div>

        <div class="donation-banner">
            <div class="donation-text">
                <h4>Support the Workforce Training Campus</h4>
                <p>Your tax-deductible contribution directly funds hands-on training tools, equipment, and resources for our students.</p>
            </div>
            <a href="https://www.paypal.com/ncp/payment/6LTBWH4TUVJYJ" target="_blank" class="paypal-direct-link">https://www.paypal.com/ncp/payment/6LTBWH4TUVJYJ</a>
        </div>

        <h2 class="section-title">Skilled Training Focus</h2>
        <div class="gallery-grid">
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1504307651254-35680f356dfd?q=80&w=600&auto=format&fit=crop" alt="African American Construction Manager Planning Site Prep">
                <div class="gallery-caption">Site Prep & Infrastructure</div>
            </div>
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1573164713988-8665fc963095?q=80&w=600&auto=format&fit=crop" alt="Minority Skilled Trade Engineering Collaboration">
                <div class="gallery-caption">Construction Management</div>
            </div>
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1581094288338-2314dddb7ece?q=80&w=600&auto=format&fit=crop" alt="African American Technical Professional Executing Ground-Up Build Features">
                <div class="gallery-caption">Ground-Up Completion</div>
            </div>
        </div>

        <div class="grid-2">
            <div class="card card-leadership">
                <div>
                    <h3>Executive Leadership</h3>
                    <ul>
                        <li><span>Todd Chavis</span> <strong>President & Director</strong></li>
                        <li><span>Lakeya R. Chavis</span> <strong>Secretary</strong></li>
                        <li><span>Anthony Moultrie</span> <strong>Director</strong></li>
                        <li><span>Tywillie Chavis</span> <strong>Director</strong></li>
                    </ul>
                </div>
                <a href="#leadership-history" class="btn btn-sm">View Leadership Backgrounds &rarr;</a>
            </div>
            
            <div class="card card-framework">
                <div>
                    <h3>Corporate Framework</h3>
                    <ul>
                        <li><span>Structure</span> <strong>Public Benefit Corporation</strong></li>
                        <li><span>Location</span> <strong>Moncks Corner, SC</strong></li>
                        <li><span>IRS Focus</span> <strong>Charitable 501(c)(3) Purpose</strong></li>
                    </ul>
                </div>
            </div>
        </div>

        <div id="leadership-history" class="history-section">
            <h2 class="section-title">Leadership Background & History</h2>
            
            <div class="history-profile">
                <h3>Todd Chavis</h3>
                <div class="title">President & Director</div>
                <p class="bio-text">Todd Chavis brings decades of professional, field-tested experience in construction management, large-scale project supervision, and quality control systems. Throughout his career, Todd has established a robust track record of guiding builds from raw site preparation and essential infrastructure layout straight through to ground-up structural completion.</p>
                <p class="bio-text">Dedicated to safety compliance and high-caliber team leadership, he envisions Inclusive Sovereignty Inc. as a direct vessel for community enrichment. By utilizing his extensive industry insights, Todd designs hands-on mentorship structures that transform the training campus into a powerhouse for student career pipelines and lasting economic self-reliance.</p>
            </div>

            <div class="history-profile">
                <h3>Lakeya R. Chavis</h3>
                <div class="title">Corporate Secretary</div>
                <p class="bio-text">Lakeya R. Chavis anchors the executive leadership group with an extensive background in organizational administration, compliance systems, and corporate communications. Her oversight guarantees seamless strategic operations across all organizational divisions, managing crucial legal, clerical, and corporate frameworks.</p>
                <p class="bio-text">Deeply invested in community revitalization, Lakeya channels her organizational strengths toward forging long-term community relationships, building strategic public benefit partnerships, and managing regional workforce outreach initiatives to reduce barriers to entry for underserved groups.</p>
            </div>
        </div>

    </div>

    <footer>
        <p><strong>Inclusive Sovereignty Inc.</strong><br>Moncks Corner, SC 29461</p>
        <p style="margin-top: 1rem; color: #4b5563;">&copy; 2026 Organized exclusively for charitable and educational purposes.</p>
    </footer>

</body>
</html>
