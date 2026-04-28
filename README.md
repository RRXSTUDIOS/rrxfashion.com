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
            --transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        /* Dark Mode Colors */
        [data-theme="dark"] {
            --bg-color: #0a0a0a;
            --text-color: #ffffff;
            --card-bg: #151515;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            transition: var(--transition);
            overflow-x: hidden;
        }

        /* Header & Theme Toggle */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            background: var(--bg-color);
            border-bottom: 1px solid rgba(128,128,128,0.1);
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.4rem;
            letter-spacing: 4px;
            font-weight: bold;
        }

        .nav-right {
            display: flex;
            align-items: center;
            gap: 25px;
        }

        .theme-toggle {
            cursor: pointer;
            background: none;
            border: 1px solid var(--text-color);
            color: var(--text-color);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.7rem;
            letter-spacing: 1px;
            transition: var(--transition);
        }

        .theme-toggle:hover {
            background: var(--text-color);
            color: var(--bg-color);
        }

        /* Hero Section with Slide Effect */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), 
                        url('https://images.unsplash.com/photo-1441984904996-e0b6ba687e04?auto=format&fit=crop&q=80&w=2070');
            background-size: cover;
            background-position: center;
            color: white;
        }

        .hero-content h1 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(3rem, 8vw, 5.5rem);
            animation: fadeInUp 1s ease-out;
        }

        /* Buttons with Animation */
        .btn {
            position: relative;
            padding: 15px 40px;
            color: white;
            text-decoration: none;
            font-size: 0.8rem;
            letter-spacing: 2px;
            border: 1px solid white;
            overflow: hidden;
            display: inline-block;
            margin-top: 20px;
            transition: var(--transition);
        }

        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: white;
            transition: var(--transition);
            z-index: -1;
        }

        .btn:hover::before { left: 0; }
        .btn:hover { color: black; transform: translateY(-3px); }

        /* Product Grid Section */
        .section { padding: 100px 8%; }
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.2rem;
            margin-bottom: 50px;
            text-align: center;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .card {
            background: var(--card-bg);
            transition: var(--transition);
            position: relative;
            border-radius: 4px;
            overflow: hidden;
        }

        .card:hover { transform: translateY(-10px); }

        .card-img {
            height: 400px;
            background-size: cover;
            background-position: center;
            transition: transform 0.8s ease;
        }

        .card:hover .card-img { transform: scale(1.1); }

        .card-info {
            padding: 20px;
            text-align: center;
        }

        .price { color: var(--accent); font-weight: bold; margin-top: 5px; }

        /* Animations */
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Responsive Mobile */
        @media (max-width: 768px) {
            nav { padding: 15px 5%; }
            .grid { grid-template-columns: 1fr 1fr; gap: 15px; }
            .card-img { height: 250px; }
            .hero-content h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX.FASHION</div>
        <div class="nav-right">
            <button class="theme-toggle" onclick="toggleTheme()" id="themeBtn">SUNLIGHT</button>
        </div>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <h1>RRX PREMIUM</h1>
            <p style="letter-spacing: 5px;">ESTABLISHED 2026</p>
            <a href="#men" class="btn">EXPLORE</a>
        </div>
    </header>

    <section class="section" id="men">
        <h2 class="section-title">Men's Collection</h2>
        <div class="grid">
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1617137968427-85924c800a22?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Premium Suit</h3>
                    <p class="price">৳ 8,500</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1550246140-5119ae4790b8?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Midnight Tee</h3>
                    <p class="price">৳ 1,200</p>
                </div>
            </div>
        </div>
    </section>

    <section class="section" id="women" style="background: var(--card-bg);">
        <h2 class="section-title">Women's Luxury</h2>
        <div class="grid">
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Silk Evening Dress</h3>
                    <p class="price">৳ 5,800</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1485230895905-ec40ba36b9bc?auto=format&fit=crop&q=80&w=400');"></div>
                <div class="card-info">
                    <h3>Woolen Overcoat</h3>
                    <p class="price">৳ 7,500</p>
                </div>
            </div>
        </div>
    </section>

    <footer style="padding: 50px; text-align: center; border-top: 1px solid rgba(128,128,128,0.1);">
        <p>© 2026 RRXFASHION.COM</p>
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
