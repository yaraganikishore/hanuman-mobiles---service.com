<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>TechNova Mobiles | Premium Store</title>

    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #0f172a;
            color: white;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
        }

        /* Navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 10%;
            background: #1e293b;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: white;
        }

        .logo span {
            color: #38bdf8;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 25px;
        }

        .nav-links a {
            text-decoration: none;
            color: #cbd5e1;
            transition: color 0.3s ease;
            font-weight: 500;
        }

        .nav-links a:hover {
            color: #38bdf8;
        }

        /* Hero Section */
        .hero {
            min-height: 60vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 40px 20px;
            background:
                linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)),
                url('https://images.unsplash.com/photo-1556656793-062ff987b48e?auto=format&fit=crop&q=80&w=1470&ixlib=rb-4.0.3')
                center/cover no-repeat;
        }

        .hero-content {
            max-width: 700px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.1rem;
            color: #e2e8f0;
        }

        .btn {
            padding: 12px 30px;
            background: #38bdf8;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 20px;
            color: #0f172a;
            transition: 0.3s ease;
        }

        .btn:hover {
            background: #0ea5e9;
            color: white;
        }

        /* Product Section */
        .products {
            padding: 50px 10%;
            text-align: center;
        }

        .products h2 {
            font-size: 2rem;
            margin-bottom: 10px;
        }

        .product-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .card {
            background: #1e293b;
            padding: 20px;
            border-radius: 15px;
            position: relative;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }

        .card img {
            width: 100%;
            max-width: 200px;
            height: 250px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .card h3 {
            margin-bottom: 8px;
            font-size: 1.2rem;
        }

        .badge {
            position: absolute;
            top: 10px;
            left: 10px;
            background: #ef4444;
            padding: 5px 10px;
            font-size: 12px;
            border-radius: 5px;
            font-weight: bold;
        }

        .price {
            font-size: 20px;
            color: #38bdf8;
            margin: 10px 0;
            font-weight: bold;
        }

        .buy-btn {
            width: 100%;
            padding: 10px;
            border: 1px solid #38bdf8;
            background: transparent;
            color: #38bdf8;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s ease;
        }

        .buy-btn:hover {
            background: #38bdf8;
            color: white;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 15px;
                padding: 20px;
            }

            .nav-links {
                flex-wrap: wrap;
                justify-content: center;
                gap: 15px;
            }

            .hero h1 {
                font-size: 2.2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .products {
                padding: 40px 20px;
            }
        }
    </style>
</head>
<body>

    <nav class="navbar">
        <div class="logo">Tech<span>Nova</span></div>
        <ul class="nav-links">
            <li><a href="#">Home</a></li>
            <li><a href="#">Shop</a></li>
            <li><a href="#">Accessories</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <h1>The Future is Calling.</h1>
            <p>Grab the latest smartphones with unbeatable deals and 2-year warranty.</p>
            <button class="btn">Shop Now</button>
        </div>
    </header>

    <section class="products">
        <h2>Featured Devices</h2>
        <div class="product-container">
            <div class="card">
                <div class="badge">New</div>
                <img src="https://via.placeholder.com/200x250" alt="Galaxy Z Fold 5" />
                <h3>Galaxy Z Fold 5</h3>
                <p class="price">$1,799.00</p>
                <button class="buy-btn">Add to Cart</button>
            </div>

            <div class="card">
                <img src="https://via.placeholder.com/200x250" alt="iPhone 15 Pro" />
                <h3>iPhone 15 Pro</h3>
                <p class="price">$999.00</p>
                <button class="buy-btn">Add to Cart</button>
            </div>

            <div class="card">
                <img src="https://via.placeholder.com/200x250" alt="Pixel 8 Pro" />
                <h3>Pixel 8 Pro</h3>
                <p class="price">$899.00</p>
                <button class="buy-btn">Add to Cart</button>
            </div>
        </div>
    </section>

</body>
</html>
