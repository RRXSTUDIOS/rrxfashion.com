<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX FASHION | Official Store</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg-color: #ffffff;
            --text-color: #111111;
            --accent: #c5a059;
            --card-bg: #f9f9f9;
            --glow: 0 0 10px rgba(197, 160, 89, 0.5);
            --transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        [data-theme="dark"] {
            --bg-color: #0a0a0a;
            --text-color: #ffffff;
            --card-bg: #151515;
            --glow: 0 0 20px rgba(197, 160, 89, 0.8);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
            text-decoration: none !important; /* নীল লিঙ্ক কালার রিমুভ করার জন্য */
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            transition: var(--transition);
            overflow-x: hidden;
        }

        /* Fixed Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 5%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            background: var(--bg-color);
            border-bottom: 1px solid rgba(128,128,128,0.1);
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.2rem;
            letter-spacing: 3px;
            font-weight: bold;
            color: var(--text-color);
        }

        /* Sunlight Button Fixed & Polished */
        .theme-toggle {
            cursor: pointer;
            background: transparent;
            border: 1px solid var(--text-color);
            color: var(--text-color);
            padding: 8px 18px;
            border-radius: 25px;
            font-size: 0.7rem;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            font-weight: 500;
            transition: var(--transition);
            outline: none;
        }

        .theme-toggle:hover {
            background: var(--text-color);
            color: var(--bg-color);
            box-shadow: var(--glow);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), 
                        url('https://images.unsplash.com/photo-1441984904996-e0b6ba687e04?auto=format&fit=crop&q=80&w=2070');
            background-size: cover;
            background-position: center;
            color: white;
            margin-top: 0; /* গ্যাপ রিমুভ করার জন্য */
        }

        .hero-content h1 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2.5rem, 7vw, 5rem);
            animation: fadeInUp 1.2s ease-out;
            letter-spacing: 5px;
            color: white;
        }

        .btn {
            position: relative;
            padding: 12px 35px;
            color: white;
            border: 1px solid white;
            display: inline-block;
            margin-top: 25px;
            transition: var(--transition);
            z-index: 1;
            background: transparent;
        }

        .btn:hover { color: black; background: white; transform: scale(1.05); }

        /* Sections */
        .section { padding: 80px 5%; }
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            margin-bottom: 40px;
            text-align: center;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .card {
            background: var(--card-bg);
            transition: var(--transition);
            border-radius: 5px;
            overflow: hidden;
        }

        .card-img {
            height: 350px;
            background-size: cover;
            background-position: center;
            transition: transform 0.8s ease;
        }

        .card:hover .card-img { transform: scale(1.08); }

        .card-info { padding: 15px; text-align: center; }

        .price { color: var(--accent); font-weight: bold; }

        /* Footer with GLOW EFFECT */
        footer {
            padding: 60px 5%;
            text-align: center;
            background: var(--bg-color);
            border-top: 1px solid rgba(128,128,128,0.1);
        }

        .footer-logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            letter-spacing: 4px;
            margin-bottom: 15px;
        }

        .copyright-glow {
            font-size: 0.75rem;
            letter-spacing: 2px;
            color: var(--accent);
            text-shadow: var(--glow);
            font-weight: 500;
            margin-top: 10px;
            display: block; /* প্রপার গ্লো এর জন্য */
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 768px) {
            .grid { grid-template-columns: 1fr 1fr; }
            .hero-content h1 { font-size: 2.2rem; }
            .card-img { height: 220px; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX.FASHION</div>
        <button class="theme-toggle" onclick="toggleTheme()" id="themeBtn">SUNLIGHT</button>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <h1>RRX PREMIUM</h1>
            <p style="letter-spacing: 5px; font-weight: 300;">THE NEW STANDARD</p>
            <a href="#men" class="btn">VIEW DROPS</a>
        </div>
    </header>

    <section class="section" id="men">
        <h2 class="section-title">Men's Select</h2>
        <div class="grid">
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1617137968427-85924c800a22?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Signature Suit</h3>
                    <p class="price">৳ 8,500</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1550246140-5119ae4790b8?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Essential Tee</h3>
                    <p class="price">৳ 1,200</p>
                </div>
            </div>
        </div>
    </section>

    <section class="section" id="women" style="background: var(--card-bg);">
        <h2 class="section-title">Women's Couture</h2>
        <div class="grid">
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Evening Silk</h3>
                    <p class="price">৳ 5,800</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1485230895905-ec40ba36b9bc?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Wool Overcoat</h3>
                    <p class="price">৳ 7,500</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-logo">RRX FASHION</div>
        <p class="copyright-glow">@2026 COPYRIGHT RRXFASHION BY RRX STUDIOS</p>
    </footer>

    <script>
        function toggleTheme() {
            const body = document.body;
            const btn = document.getElementById('themeBtn');
            if (body.getAttribute('data-theme') === 'dark') {
                body.removeAttribute('data-theme');
                btn.innerText = "SUNLIGHT";
            } else {
                body.setAttribute('data-theme', 'dark');
                btn.innerText = "DARKNESS";
            }
        }
    </script>
</body>
</html>
