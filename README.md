<!DOCTYPE html>
<html>

<head> </head>

<body>

    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Food Corner | Delicious Food</title>

        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

        <style>
            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
                scroll-behavior: smooth;
            }

            body {
                font-family: 'Poppins', sans-serif;
                color: #333;
            }

            /* Navigation */
            header {
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 20px 8%;
                background: white;
                position: sticky;
                top: 0;
                z-index: 100;
                box-shadow: 0 2px 10px #0001;
            }

            .logo {
                font-size: 28px;
                font-weight: 700;
                color: #e63946;
            }

            nav a {
                text-decoration: none;
                color: #333;
                margin-left: 25px;
                font-weight: 500;
            }

            nav a:hover {
                color: #e63946;
            }

            /* Hero Section */
            .hero {
                min-height: 85vh;
                display: flex;
                align-items: center;
                padding: 60px 8%;
                background:
                    linear-gradient(90deg, #000b, #0003),
                    url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1800&q=85') center/cover;
                color: white;
            }

            .hero-content {
                max-width: 650px;
            }

            .hero h1 {
                font-size: clamp(38px, 6vw, 65px);
                line-height: 1.2;
                margin-bottom: 20px;
            }

            .hero p {
                font-size: 18px;
                margin-bottom: 30px;
            }

            .btn {
                display: inline-block;
                background: #e63946;
                color: white;
                padding: 13px 28px;
                border-radius: 6px;
                text-decoration: none;
                transition: 0.3s;
            }

            .btn:hover {
                background: #c82333;
                transform: translateY(-2px);
            }

            /* General Sections */
            section {
                padding: 75px 8%;
            }

            .section-title {
                text-align: center;
                font-size: 35px;
                margin-bottom: 40px;
            }

            .section-title span {
                color: #e63946;
            }

            /* About */
            .about {
                display: flex;
                align-items: center;
                gap: 45px;
            }

            .about img {
                width: 50%;
                border-radius: 12px;
                object-fit: cover;
            }

            .about-content {
                flex: 1;
            }

            .about-content h2 {
                font-size: 32px;
                margin-bottom: 20px;
            }

            .about-content p {
                line-height: 1.8;
                margin-bottom: 25px;
            }

            /* Menu */
            .menu {
                background: #fff8f0;
            }

            .food-container {
                display: grid;
                grid-template-columns: repeat(3, 1fr);
                gap: 25px;
            }

            .food-card {
                background: white;
                border-radius: 12px;
                overflow: hidden;
                box-shadow: 0 4px 18px #0001;
                transition: 0.3s;
            }

            .food-card:hover {
                transform: translateY(-7px);
                box-shadow: 0 8px 25px #0002;
            }

            .food-card img {
                width: 100%;
                height: 220px;
                object-fit: cover;
            }

            .food-info {
                padding: 20px;
            }

            .food-info h3 {
                margin-bottom: 10px;
            }

            .food-info p {
                color: #666;
                font-size: 14px;
                margin-bottom: 15px;
            }

            .price {
                color: #e63946;
                font-size: 20px;
                font-weight: 700;
            }

            /* Contact */
            .contact {
                text-align: center;
            }

            .contact p {
                margin-bottom: 25px;
            }

            footer {
                background: #222;
                color: white;
                text-align: center;
                padding: 25px;
            }

            /* Mobile Responsive */
            @media (max-width: 768px) {
                header {
                    flex-direction: column;
                    gap: 15px;
                }

                nav a {
                    margin: 0 7px;
                    font-size: 14px;
                }

                .hero {
                    min-height: 70vh;
                }

                .about {
                    flex-direction: column;
                }

                .about img {
                    width: 100%;
                }

                .food-container {
                    grid-template-columns: 1fr;
                }

                .section-title {
                    font-size: 28px;
                }
            }
        </style>
    </head>

    <body>

        <!-- Navigation -->
        <header>
            <div class="logo">Food Corner</div>

            <nav>
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#menu">Menu</a>
                <a href="#contact">Contact</a>
            </nav>
        </header>

        <!-- Home -->
        <section class="hero" id="home">
            <div class="hero-content">
                <h1>Delicious Food,<br>Happy Moments</h1>
                <p>
                    Enjoy freshly prepared meals made with love.
                    Discover your favourite flavours at Food Corner.
                </p>
                <a href="#menu" class="btn">Explore Our Menu</a>
            </div>
        </section>

        <!-- About -->
        <section id="about">
            <h2 class="section-title">About <span>Us</span></h2>

            <div class="about">
                <img src="https://images.unsplash.com/photo-1555396273-367ea4eb4db5?auto=format&fit=crop&w=900&q=80" alt="Restaurant dining area">

                <div class="about-content">
                    <h2>Welcome to Food Corner</h2>
                    <p>
                        We believe great food brings people together.
                        Our restaurant serves delicious meals prepared
                        with fresh ingredients and care.
                    </p>
                    <p>
                        Whether you're enjoying a family dinner or
                        catching up with friends, we're happy to serve you.
                    </p>
                    <a href="#contact" class="btn">Contact Us</a>
                </div>
            </div>
        </section>

        <!-- Popular Dishes -->
        <section class="menu" id="menu">
            <h2 class="section-title">Popular <span>Dishes</span></h2>

            <div class="food-container">

                <div class="food-card">
                    <img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?auto=format&fit=crop&w=700&q=80" alt="Delicious pizza">
                    <div class="food-info">
                        <h3>Cheese Pizza</h3>
                        <p>Freshly baked pizza topped with cheese and herbs.</p>
                        <div class="price">₹199</div>
                    </div>
                </div>

                <div class="food-card">
                    <img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=700&q=80" alt="Burger with fresh toppings">
                    <div class="food-info">
                        <h3>Classic Burger</h3>
                        <p>A tasty burger with fresh vegetables and sauce.</p>
                        <div class="price">₹149</div>
                    </div>
                </div>

                <div class="food-card">
                    <img src="https://images.unsplash.com/photo-1513104890138-7c749659a591?auto=format&fit=crop&w=700&q=80" alt="Freshly baked pizza">
                    <div class="food-info">
                        <h3>Special Pizza</h3>
                        <p>A delicious combination of flavours and toppings.</p>
                        <div class="price">₹249</div>
                    </div>
                </div>

            </div>
        </section>

        <!-- Contact -->
        <section class="contact" id="contact">
            <h2 class="section-title">Contact <span>Us</span></h2>
            25 Main street, Chennai <br />
            8890143567<br />
            foodcorner@example.com

            <p>We would love to hear from you!</p>
            <a href="mailto:hello@foodcorner.example" class="btn">
                Send Us an Email
            </a>
        </section>

        <!-- Footer -->
        <footer>
            <p>&copy; 2026 Food Corner. All rights reserved.</p>
        </footer>

    </body>

    </html>

</body>

</html>












@import url('https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap');

:root {
    --wine: #5b201e;
    --wine-dark: #401614;
    --cream: #faf6f1;
    --yellow: #ffc928;
    --text: #332b29;
    --muted: #756a66;
    --white: #fff;
    --shadow: 0 8px 25px rgba(53, 30, 23, .10);
}

* {
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 82px;
}

body {
    margin: 0;
    background: var(--cream);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    line-height: 1.6;
}

img {
    display: block;
    max-width: 100%;
}

a {
    color: inherit;
    text-decoration: none;
}

.container {
    width: min(1100px, calc(100% - 40px));
    margin-inline: auto;
}

.site-header {
    background: var(--wine);
    color: var(--white);
    position: sticky;
    top: 0;
    z-index: 20;
    box-shadow: 0 2px 12px #32110f20;
}

.navbar {
    min-height: 64px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 24px;
}

.brand {
    font-family: 'Poppins', sans-serif;
    font-weight: 800;
    font-size: 1.25rem;
    letter-spacing: -.5px;
}

.brand span {
    color: var(--yellow);
    margin-left: 4px;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 30px;
    list-style: none;
    margin: 0;
    padding: 0;
}

.nav-links a {
    font-size: .92rem;
    font-weight: 600;
    opacity: .92;
    transition: color .2s;
}

.nav-links a:hover {
    color: var(--yellow);
}

.menu-toggle {
    display: none;
    border: 0;
    background: transparent;
    color: white;
    font-size: 1.7rem;
    cursor: pointer;
}

.hero {
    min-height: 440px;
    margin-top: 28px;
    display: grid;
    place-items: center;
    position: relative;
    overflow: hidden;
    border-radius: 5px;
    background: #24433e center 48%/cover no-repeat;
}

.hero {
    background-image: url('https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?auto=format&fit=crop&w=1800&q=90');
}

.hero-overlay {
    position: absolute;
    inset: 0;
    background: linear-gradient(90deg, rgba(8, 28, 26, .70), rgba(8, 28, 26, .42));
}

.hero-content {
    position: relative;
    z-index: 1;
    text-align: center;
    color: white;
    max-width: 680px;
    padding: 60px 24px;
}

.eyebrow {
    color: var(--wine);
    letter-spacing: 2px;
    font-size: .68rem;
    font-weight: 800;
    margin: 0 0 9px;
}

.hero .eyebrow {
    color: var(--yellow);
}

h1,
h2,
h3 {
    font-family: 'Poppins', sans-serif;
    line-height: 1.2;
}

.hero h1 {
    font-size: clamp(2rem, 5vw, 3.3rem);
    margin: 0 0 15px;
    font-weight: 800;
}

.hero-content>p:not(.eyebrow) {
    max-width: 490px;
    margin: 0 auto 23px;
    color: #f5f5f5;
    font-size: .98rem;
}

.button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    padding: 11px 23px;
    border-radius: 30px;
    background: var(--yellow);
    color: #35220a;
    font-weight: 800;
    font-size: .9rem;
    box-shadow: 0 4px 12px #0002;
    transition: transform .2s, background .2s;
}

.button:hover {
    transform: translateY(-2px);
    background: #ffda58;
}

.about-section {
    padding-top: 35px;
}

.about-card {
    background: var(--white);
    border-radius: 14px;
    box-shadow: var(--shadow);
    padding: 25px;
    display: grid;
    grid-template-columns: .9fr 1.1fr;
    gap: 34px;
    align-items: center;
}

.about-image {
    min-height: 265px;
    border-radius: 10px;
    background: url('https://images.unsplash.com/photo-1414235077428-338989a2e8c0?auto=format&fit=crop&w=1000&q=85') center/cover;
}

.about-copy h2,
.section-heading h2,
.contact-inner h2 {
    color: var(--wine);
    margin: 0 0 14px;
    font-size: clamp(1.55rem, 3vw, 2rem);
}

.about-copy p:not(.eyebrow) {
    color: var(--muted);
    font-size: .95rem;
    margin: 0 0 12px;
}

.text-link {
    display: inline-block;
    margin-top: 5px;
    color: var(--wine);
    font-weight: 800;
    font-size: .9rem;
}

.text-link:hover {
    color: #9a3b31;
}

.menu-section {
    padding-block: 65px 72px;
}

.section-heading {
    text-align: center;
    margin-bottom: 28px;
}

.section-heading>p:last-child {
    color: var(--muted);
    margin: 0;
}

.dish-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 22px;
}

.dish-card {
    background: white;
    border-radius: 13px;
    overflow: hidden;
    box-shadow: var(--shadow);
    transition: transform .2s;
}

.dish-card:hover {
    transform: translateY(-5px);
}

.dish-card img {
    width: 100%;
    height: 205px;
    object-fit: cover;
}

.dish-info {
    padding: 18px;
    position: relative;
}

.dish-info h3 {
    color: var(--wine);
    font-size: 1.1rem;
    margin: 0 0 6px;
}

.dish-info p {
    color: var(--muted);
    font-size: .9rem;
    margin: 0 0 12px;
}

.price {
    color: var(--wine);
    font-weight: 800;
}

.contact-section {
    background: #f0e5dc;
    padding: 45px 0;
}

.contact-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 25px;
}

.contact-inner h2 {
    margin-bottom: 8px;
}

.contact-inner p:not(.eyebrow) {
    color: var(--muted);
    margin: 0;
}

.footer {
    background: var(--wine-dark);
    color: #f8eee8;
    text-align: center;
    padding: 17px 20px;
    font-size: .85rem;
}

.footer p {
    margin: 0;
}

.footer span {
    color: var(--yellow);
}

@media (max-width: 700px) {
    .container {
        width: min(100% - 28px, 560px);
    }

    .navbar {
        min-height: 58px;
    }

    .menu-toggle {
        display: block;
    }

    .nav-links {
        display: none;
        position: absolute;
        top: 58px;
        left: 0;
        right: 0;
        padding: 16px 22px 20px;
        background: var(--wine);
        flex-direction: column;
        align-items: flex-start;
        gap: 14px;
        box-shadow: 0 8px 12px #0002;
    }

    .nav-links.open {
        display: flex;
    }

    .hero {
        min-height: 390px;
        margin-top: 16px;
    }

    .hero-content {
        padding: 50px 18px;
    }

    .about-card {
        grid-template-columns: 1fr;
        padding: 17px;
        gap: 20px;
    }

    .about-image {
        min-height: 220px;
    }

    .menu-section {
        padding-block: 48px;
    }

    .dish-grid {
        grid-template-columns: 1fr;
        gap: 18px;
    }

    .dish-card img {
        height: 230px;
    }

    .contact-inner {
        align-items: flex-start;
        flex-direction: column;
    }
}
