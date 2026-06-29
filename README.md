<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-Football Championship 2026</title>
    <style>
        /* CSS Variables for Consistent Color Palette */
        :root {
            --bg-color: #0d1117;
            --surface-color: #161b22;
            --primary-accent: #00ff88;
            --text-main: #c9d1d9;
            --text-light: #ffffff;
            --font-main: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        /* Base Reset & Box Sizing (Prevents Element Overlap) */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: var(--font-main);
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Typography */
        h1, h2, h3 {
            color: var(--text-light);
            font-weight: 700;
        }
        
        h1 { font-size: 3rem; margin-bottom: 1rem; }
        h2 { font-size: 2.2rem; margin-bottom: 1.5rem; text-align: center; }
        h3 { font-size: 1.5rem; margin-bottom: 1rem; }
        p { font-size: 1.1rem; }

        /* Fixed / Sticky Navigation Bar */
        nav {
            position: sticky;
            top: 0;
            background-color: rgba(22, 27, 34, 0.95);
            backdrop-filter: blur(10px);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 5%;
            z-index: 1000;
            border-bottom: 1px solid #30363d;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-accent);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-light);
            font-weight: 600;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--primary-accent);
        }

        /* Hero Section */
        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 8rem 5%;
            min-height: 70vh;
            background: linear-gradient(180deg, rgba(13,17,23,0) 0%, var(--bg-color) 100%), 
                        url('https://images.unsplash.com/photo-1542751371-adc38448a05e?q=80&w=2070&auto=format&fit=crop') center/cover;
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 600px;
            margin-bottom: 2.5rem;
            color: #e6edf3;
        }

        .cta-btn {
            display: inline-block;
            background-color: var(--primary-accent);
            color: #000;
            padding: 1rem 2.5rem;
            font-size: 1.2rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 5px;
            text-transform: uppercase;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .cta-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 255, 136, 0.4);
        }

        /* Content Sections Layout (Flexbox) */
        section {
            padding: 5rem 5%;
        }

        .features-container {
            display: flex;
            justify-content: space-between;
            gap: 2rem;
            flex-wrap: wrap; /* Ensures responsiveness */
        }

        .feature-card {
            background-color: var(--surface-color);
            flex: 1;
            min-width: 300px;
            padding: 2.5rem;
            border-radius: 8px;
            text-align: center;
            border: 1px solid #30363d;
            transition: border-color 0.3s ease;
        }

        .feature-card:hover {
            border-color: var(--primary-accent);
        }

        /* About / Details Section */
        .about-section {
            background-color: var(--surface-color);
            text-align: center;
            border-top: 1px solid #30363d;
            border-bottom: 1px solid #30363d;
        }

        .about-content {
            max-width: 800px;
            margin: 0 auto;
        }

        /* Footer */
        footer {
            background-color: #010409;
            text-align: center;
            padding: 3rem 5%;
        }

        .social-links {
            margin-top: 1.5rem;
            display: flex;
            justify-content: center;
            gap: 1.5rem;
        }

        .social-links a {
            color: var(--primary-accent);
            text-decoration: none;
            font-weight: bold;
        }

        /* Responsive Layout - Mobile Breakpoint */
        @media (max-width: 768px) {
            nav {
                flex-direction: column;
                gap: 1rem;
                padding: 1rem;
            }
            
            h1 { font-size: 2.2rem; }
            h2 { font-size: 1.8rem; }
            
            .hero {
                padding: 5rem 5%;
            }

            .features-container {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">Cup Series</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#format">Tournament Format</a></li>
            <li><a href="#details">Event Details</a></li>
        </ul>
    </nav>

    <header class="hero" id="home">
        <h1>Ultimate E-Football Showdown</h1>
        <p>Step onto the virtual pitch and prove your skills. Compete against top players, climb the knockout brackets, and claim the championship title.</p>
        <a href="#register" class="cta-btn">Register Now</a>
    </header>

    <section id="format">
        <h2>Tournament Features</h2>
        <div class="features-container">
            <div class="feature-card">
                <h3>Knockout Format</h3>
                <p>High stakes, single-elimination bracket system. One mistake can cost you the trophy. Bring your best starting XI.</p>
            </div>
            <div class="feature-card">
                <h3>Live Scorecards</h3>
                <p>Track player progression in real-time. Our custom frontend ensures you never miss a match result or bracket update.</p>
            </div>
            <div class="feature-card">
                <h3>Prize Pool</h3>
                <p>Compete for the ultimate prize. The top three finalists will receive exclusive rewards and the championship trophy.</p>
            </div>
        </div>
    </section>

    <section id="details" class="about-section">
        <div class="about-content">
            <h2>About The Event</h2>
            <p>Organized for the competitive community, this tournament brings together the best local talent for an unforgettable weekend of digital football. Please ensure your setup is updated to the latest patch before entering the lobby. Match rules, team restrictions, and lobby codes will be sent to registered players via email.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 E-Football Championship. All rights reserved.</p>
        <div class="social-links">
            <a href="#">Discord</a>
            <a href="#">Twitch</a>
            <a href="#">Instagram</a>
            <a href="#">Contact Support</a>
        </div>
    </footer>

</body>
</html>
