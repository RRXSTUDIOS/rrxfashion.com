<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX FASHION | Premium Clothing Store</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg-color: #ffffff;
            --brand-black: #0f0f0f;
            --gold-accent: #c5a059; /* প্রিমিয়াম লুকের জন্য গোল্ডেন টাচ */
            --light-gray: #f4f4f4;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--bg-color);
            color: var(--brand-black);
            overflow-x: hidden;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(5px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid #eee;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            letter-spacing: 5px;
            font-weight: bold;
            color: var(--brand-black);
            text-transform: uppercase;
        }

        .logo span {
            color: var(--gold-accent);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li { margin-left: 30px; }

        nav ul li a {
            text-decoration: none;
            color: var(--brand-black);
            font-size: 0.75rem;
            font-weight: 500;
            letter-spacing: 2px;
            transition: 0.3s;
        }

        nav ul li a:hover { color: var(--gold-accent); }

        /* Hero */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), 
                        url('https://images.unsplash.com/photo-1490481651871-ab68de25d43d?auto=format&fit=crop&q=80&w=2070') center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 5rem;
            letter-spacing: 8px;
            margin-bottom: 10px;
        }

        .hero p {
            letter-spacing: 4px;
            font-weight: 300;
            margin-bottom: 30px;
            text-transform: uppercase;
        }

        .btn {
            padding: 15px 45px;
            border: 1px solid white;
            background: transparent;
            color: white;
            text-decoration: none;
            font-size: 0.8rem;
            letter-spacing: 2px;
            transition: 0.4s;
        }

        .btn:hover {
            background: white;
            color: black;
        }

        /* Products Section */
        .products {
            padding: 100px 8%;
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-header h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            letter-spacing: 3px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .card {
            position: relative;
            cursor: pointer;
            overflow: hidden;
        }

        .card-img {
            height: 500px;
            background-color: var(--light-gray);
            background-size: cover;
            background-position: center;
            transition: transform 0.5s;
        }

        .card:hover .card-img {
            transform: scale(1.05);
        }

        .card-info {
            padding-top: 20px;
            text-align: center;
        }

        .card-info h3 {
            font-size: 0.9rem;
            letter-spacing: 1px;
            margin-bottom: 5px;
            text-transform: uppercase;
        }

        .price {
            color: var(--gold-accent);
            font-weight: 500;
        }

        /* Footer */
        footer {
            padding: 80px 8%;
            background: #111;
            color: white;
            text-align: center;
        }

        .footer-logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            letter-spacing: 4px;
            margin-bottom: 30px;
        }

        .copyright {
            font-size: 0.7rem;
            color: #555;
            margin-top: 40px;
            letter-spacing: 1px;
        }

        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            nav ul { display: none; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX<span>.</span>FASHION</div>
        <ul>
            <li><a href="#">COLLECTIONS</a></li>
            <li><a href="#">MEN</a></li>
            <li><a href="#">WOMEN</a></li>
            <li><a href="#">CONTACT</a></li>
        </ul>
    </nav>

    <header class="hero">
        <p>Redefining Elegance</p>
        <h1>RRX FASHION</h1>
        <a href="#shop" class="btn">VIEW COLLECTION</a>
    </header>

    <section class="products" id="shop">
        <div class="section-header">
            <h2>NEW ARRIVALS</h2>
        </div>
        <div class="grid">
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1618354691373-d851c5c3a990?auto=format&fit=crop&q=80&w=400x500');"></div>
                <div class="card-info">
                    <h3>Midnight Premium Tee</h3>
                    <p class="price">৳ 1,490</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1551028719-00167b16eac5?auto=format&fit=crop&q=80&w=400x500');"></div>
                <div class="card-info">
                    <h3>Aesthetic Leather Biker</h3>
                    <p class="price">৳ 4,200</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1620799140408-edc6dcb6d633?auto=format&fit=crop&q=80&w=400x500');"></div>
                <div class="card-info">
                    <h3>Minimalist White Sweatshirt</h3>
                    <p class="price">৳ 2,150</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-logo">RRX FASHION</div>
        <p style="font-size: 0.8rem; letter-spacing: 2px;">Premium Quality | Timeless Design</p>
        <p class="copyright">© 2026 RRXFASHION.COM | ALL RIGHTS RESERVED.</p>
    </footer>

</body>
</html>
