<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inclusive Sovereignty Inc.</title>
    <style>
        :root {
            --primary: #1e3a8a;
            --secondary: #f59e0b;
            --dark: #1f2937;
            --light: #f9fafb;
            --white: #ffffff;
            --gray: #6b7280;
            --accent-green: #10b981;
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
            /* Hero background image optimized to feature African American construction leadership */
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
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            margin-bottom: 2rem;
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
            box-shadow: 0 2px 4px rgba(0,0,0,0.02);
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
        }
        .card {
            background: var(--white);
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        .card h3 {
            margin-bottom: 1rem;
            color: var(--primary);
        }
        .card ul {
            list-style: none;
        }
        .card ul li {
            padding: 0.5rem 0;
            border-bottom: 1px solid #e5e7eb;
            display: flex;
            justify-content: space-between;
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
            transition: background
