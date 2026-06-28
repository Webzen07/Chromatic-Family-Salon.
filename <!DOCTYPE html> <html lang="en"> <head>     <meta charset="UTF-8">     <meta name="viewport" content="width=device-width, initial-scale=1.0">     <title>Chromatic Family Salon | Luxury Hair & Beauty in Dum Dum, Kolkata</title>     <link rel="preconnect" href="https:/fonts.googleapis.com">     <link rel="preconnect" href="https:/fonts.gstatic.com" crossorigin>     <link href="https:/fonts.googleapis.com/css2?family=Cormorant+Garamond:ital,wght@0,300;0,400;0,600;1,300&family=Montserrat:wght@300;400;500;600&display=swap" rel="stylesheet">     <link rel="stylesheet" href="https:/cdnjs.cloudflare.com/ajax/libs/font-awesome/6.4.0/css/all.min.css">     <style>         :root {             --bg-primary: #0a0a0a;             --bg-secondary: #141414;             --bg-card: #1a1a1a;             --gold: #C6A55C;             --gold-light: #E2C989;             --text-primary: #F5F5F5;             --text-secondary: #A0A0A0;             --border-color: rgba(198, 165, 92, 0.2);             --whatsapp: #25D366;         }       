<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chromatic Family Salon | Luxury Hair & Beauty in Dum Dum, Kolkata</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --bg-primary: #0a0a0a;
            --bg-secondary: #141414;
            --bg-card: #1a1a1a;
            --gold: #C6A55C;
            --gold-light: #E2C989;
            --text-primary: #F5F5F5;
            --text-secondary: #A0A0A0;
            --border-color: rgba(198, 165, 92, 0.2);
            --whatsapp: #25D366;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--bg-primary);
            color: var(--text-primary);
            line-height: 1.6;
            overflow-x: hidden;
        }

        h1, h2, h3, h4 {
            font-family: 'Cormorant Garamond', serif;
            font-weight: 400;
        }

        /* --- Utility & Animations --- */
        .reveal {
            opacity: 0;
            transform: translateY(40px);
            transition: all 1s cubic-bezier(0.5, 0, 0, 1);
        }

        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }

        .section-subtitle {
            font-family: 'Montserrat', sans-serif;
            font-size: 0.75rem;
            font-weight: 500;
            letter-spacing: 4px;
            text-transform: uppercase;
            color: var(--gold);
            margin-bottom: 1rem;
            display: block;
        }

        .section-title {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        .btn-premium {
            display: inline-block;
            padding: 14px 36px;
            border: 1px solid var(--gold);
            color: var(--gold);
            text-decoration: none;
            font-size: 0.8rem;
            font-weight: 500;
            letter-spacing: 2px;
            text-transform: uppercase;
            transition: all 0.4s ease;
            background: transparent;
            cursor: pointer;
        }

        .btn-premium:hover {
            background: var(--gold);
            color: var(--bg-primary);
        }

        .btn-filled {
            background: var(--gold);
            color: var(--bg-primary);
        }

        .btn-filled:hover {
            background: var(--gold-light);
            border-color: var(--gold-light);
        }

        /* --- Navigation --- */
        header {
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            padding: 1.5rem 5%;
            transition: all 0.4s ease;
            background: transparent;
        }

        header.scrolled {
            background: rgba(10, 10, 10, 0.95);
            backdrop-filter: blur(10px);
            padding: 1rem 5%;
            border-bottom: 1px solid var(--border-color);
        }

        nav {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.8rem;
            color: var(--text-primary);
            text-decoration: none;
            letter-spacing: 1px;
        }

        .logo span {
            color: var(--gold);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2.5rem;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-secondary);
            font-size: 0.8rem;
            font-weight: 400;
            letter-spacing: 2px;
            text-transform: uppercase;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--gold);
        }

        .menu-toggle {
            display: none;
            font-size: 1.2rem;
            cursor: pointer;
            color: var(--text-primary);
        }

        /* --- HERO SECTION --- */
        .hero {
            min-height: 100vh;
            display: grid;
            grid-template-columns: 1.1fr 1fr;
            align-items: center;
            padding: 0 5%;
            position: relative;
            overflow: hidden;
            background: var(--bg-primary);
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 20% 50%, rgba(198, 165, 92, 0.08) 0%, transparent 50%);
            pointer-events: none;
        }

        .hero-text {
            position: relative;
            z-index: 2;
            padding-right: 3rem;
            animation: fadeInLeft 1.2s ease;
        }

        .hero-text .section-subtitle {
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .hero-text .section-subtitle::before {
            content: '';
            width: 40px;
            height: 1px;
            background: var(--gold);
        }

        .hero-text h1 {
            font-size: 5rem;
            font-weight: 300;
            line-height: 1.05;
            margin-bottom: 1.5rem;
            color: var(--text-primary);
        }

        .hero-text h1 .accent {
            color: var(--gold);
            font-style: italic;
            display: inline-block;
            min-width: 280px;
            position: relative;
        }

        .hero-text p {
            font-size: 1.05rem;
            color: var(--text-secondary);
            font-weight: 300;
            margin-bottom: 2.5rem;
            max-width: 500px;
            line-height: 1.8;
        }

        .hero-cta {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .hero-image-wrapper {
            position: relative;
            height: 85vh;
            max-height: 700px;
            animation: fadeInRight 1.2s ease;
        }

        .hero-image {
            width: 100%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1560066984-138dadb4c035?auto=format&fit=crop&w=900&q=80') center/cover no-repeat;
            position: relative;
            z-index: 2;
        }

        .hero-image-wrapper::before {
            content: '';
            position: absolute;
            top: 30px;
            right: -30px;
            width: 100%;
            height: 100%;
            border: 1px solid var(--gold);
            z-index: 1;
        }

        .hero-image-wrapper::after {
            content: 'EST. DUM DUM';
            position: absolute;
            bottom: -20px;
            left: -20px;
            background: var(--bg-primary);
            color: var(--gold);
            padding: 1rem 1.5rem;
            font-size: 0.75rem;
            letter-spacing: 4px;
            border: 1px solid var(--gold);
            z-index: 3;
            font-family: 'Montserrat', sans-serif;
        }

        .scroll-indicator {
            position: absolute;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            color: var(--gold);
            font-size: 0.7rem;
            letter-spacing: 3px;
            text-transform: uppercase;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            animation: bounce 2s infinite;
            z-index: 5;
        }

        .scroll-indicator::after {
            content: '';
            width: 1px;
            height: 40px;
            background: var(--gold);
        }

        /* --- Sections General --- */
        section {
            padding: 8rem 5%;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .text-center {
            text-align: center;
        }

        /* --- Philosophy / About --- */
        .philosophy-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 5rem;
            align-items: center;
        }

        .philosophy-image {
            height: 600px;
            background: url('https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?auto=format&fit=crop&w=800&q=80') center/cover no-repeat;
            position: relative;
        }

        .philosophy-image::before {
            content: '';
            position: absolute;
            top: 20px;
            left: 20px;
            right: -20px;
            bottom: -20px;
            border: 1px solid var(--gold);
            z-index: -1;
        }

        .philosophy-text p {
            color: var(--text-secondary);
            font-weight: 300;
            margin-bottom: 1.5rem;
            font-size: 1.05rem;
        }

        /* --- Services --- */
        #services {
            background: var(--bg-secondary);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
            margin-top: 4rem;
        }

        .service-card {
            background: var(--bg-card);
            padding: 3rem 2rem;
            text-align: center;
            border: 1px solid transparent;
            transition: all 0.5s ease;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background: var(--gold);
            transform: scaleX(0);
            transition: transform 0.5s ease;
        }

        .service-card:hover {
            border-color: var(--border-color);
            transform: translateY(-10px);
        }

        .service-card:hover::before {
            transform: scaleX(1);
        }

        .service-card i {
            font-size: 2rem;
            color: var(--gold);
            margin-bottom: 1.5rem;
        }

        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .service-card p {
            color: var(--text-secondary);
            font-size: 0.9rem;
            font-weight: 300;
        }

        /* --- Gallery --- */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: repeat(2, 300px);
            gap: 1.5rem;
            margin-top: 4rem;
        }

        .gallery-item {
            overflow: hidden;
            position: relative;
            cursor: pointer;
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.8s ease;
            filter: grayscale(20%);
        }

        .gallery-item:hover img {
            transform: scale(1.1);
            filter: grayscale(0%);
        }

        .gallery-item:nth-child(1) {
            grid-row: span 2;
        }

        /* --- Contact --- */
        #contact {
            background: var(--bg-secondary);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1.5fr;
            gap: 4rem;
            margin-top: 4rem;
        }

        .contact-details {
            display: flex;
            flex-direction: column;
            gap: 2.5rem;
        }

        .contact-item h4 {
            font-size: 1.2rem;
            color: var(--gold);
            margin-bottom: 0.5rem;
            font-family: 'Montserrat', sans-serif;
            font-weight: 500;
            letter-spacing: 1px;
            text-transform: uppercase;
            font-size: 0.8rem;
        }

        .contact-item p, .contact-item a {
            color: var(--text-secondary);
            font-weight: 300;
            text-decoration: none;
            font-size: 1.1rem;
            transition: color 0.3s;
        }

        .contact-item a:hover {
            color: var(--gold);
        }

        .map-container {
            height: 100%;
            min-height: 400px;
            border: 1px solid var(--border-color);
            filter: grayscale(80%) invert(92%) contrast(83%);
        }

        .map-container iframe {
            width: 100%;
            height: 100%;
            border: 0;
        }

        /* --- Footer --- */
        footer {
            background: var(--bg-primary);
            padding: 3rem 5%;
            border-top: 1px solid var(--border-color);
            text-align: center;
        }

        .footer-logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2rem;
            color: var(--text-primary);
            margin-bottom: 1rem;
        }

        .footer-logo span { color: var(--gold); }

        .social-links {
            margin: 1.5rem 0;
        }

        .social-links a {
            color: var(--text-secondary);
            font-size: 1.2rem;
            margin: 0 15px;
            transition: all 0.3s;
        }

        .social-links a:hover {
            color: var(--gold);
            transform: translateY(-3px);
        }

        footer p {
            color: var(--text-secondary);
            font-size: 0.8rem;
            letter-spacing: 1px;
        }

        /* --- FLOATING WHATSAPP BUTTON --- */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 60px;
            height: 60px;
            background: var(--whatsapp);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            text-decoration: none;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.4);
            z-index: 999;
            transition: all 0.3s ease;
            animation: pulse 2s infinite;
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 30px rgba(37, 211, 102, 0.6);
        }

        .whatsapp-float .tooltip {
            position: absolute;
            right: 75px;
            background: var(--bg-card);
            color: var(--text-primary);
            padding: 8px 16px;
            border-radius: 6px;
            font-size: 0.8rem;
            white-space: nowrap;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.3s;
            border: 1px solid var(--border-color);
        }

        .whatsapp-float:hover .tooltip {
            opacity: 1;
        }

        /* --- Animations --- */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeInLeft {
            from { opacity: 0; transform: translateX(-40px); }
            to { opacity: 1; transform: translateX(0); }
        }

        @keyframes fadeInRight {
            from { opacity: 0; transform: translateX(40px); }
            to { opacity: 1; transform: translateX(0); }
        }

        @keyframes pulse {
            0% { box-shadow: 0 5px 20px rgba(37, 211, 102, 0.4), 0 0 0 0 rgba(37, 211, 102, 0.6); }
            70% { box-shadow: 0 5px 20px rgba(37, 211, 102, 0.4), 0 0 0 20px rgba(37, 211, 102, 0); }
            100% { box-shadow: 0 5px 20px rgba(37, 211, 102, 0.4), 0 0 0 0 rgba(37, 211, 102, 0); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateX(-50%) translateY(0); }
            50% { transform: translateX(-50%) translateY(-10px); }
        }

        @keyframes slideUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* --- Responsive --- */
        @media (max-width: 1024px) {
            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding-top: 120px;
            }
            .hero-text { padding-right: 0; margin-bottom: 3rem; }
            .hero-text .section-subtitle { justify-content: center; }
            .hero-text .section-subtitle::before { display: none; }
            .hero-text p { margin-left: auto; margin-right: auto; }
            .hero-cta { justify-content: center; }
            .hero-image-wrapper { height: 400px; max-height: 400px; }
            .services-grid { grid-template-columns: repeat(2, 1fr); }
            .gallery-grid {
                grid-template-columns: repeat(2, 1fr);
                grid-template-rows: auto;
            }
            .gallery-item:nth-child(1) { grid-row: span 1; }
        }

        @media (max-width: 768px) {
            .menu-toggle { display: block; }
            .nav-links {
                position: fixed;
                top: 0;
                right: -100%;
                width: 70%;
                height: 100vh;
                background: var(--bg-secondary);
                flex-direction: column;
                justify-content: center;
                align-items: center;
                transition: right 0.4s ease;
                border-left: 1px solid var(--border-color);
            }
            .nav-links.active { right: 0; }
            
            .hero-text h1 { font-size: 3rem; }
            .hero-text h1 .accent { min-width: auto; }
            .section-title { font-size: 2.2rem; }
            
            .philosophy-grid, .contact-grid {
                grid-template-columns: 1fr;
                gap: 3rem;
            }
            .philosophy-image { height: 400px; }
            .services-grid { grid-template-columns: 1fr; }
            .gallery-grid { grid-template-columns: 1fr; }
            .hero-image-wrapper::before { display: none; }
            .hero-image-wrapper::after { display: none; }
            .scroll-indicator { display: none; }
            
            .whatsapp-float { width: 55px; height: 55px; font-size: 1.6rem; bottom: 20px; right: 20px; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header id="navbar">
        <nav>
            <a href="#" class="logo">Chromatic <span>Family</span></a>
            <ul class="nav-links" id="navLinks">
                <li><a href="#home">Home</a></li>
                <li><a href="#philosophy">Philosophy</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="https://wa.me/919163499293?text=Hi%20Chromatic%20Family%20Salon!%20%F0%9F%91%8B%20I'd%20like%20to%20book%20an%20appointment.%20Can%20you%20help%20me%20with%20available%20slots%3F" class="book-trigger" target="_blank" style="color: var(--gold);">Book Now</a></li>
            </ul>
            <div class="menu-toggle" id="menuToggle">
                <i class="fas fa-bars"></i>
            </div>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div class="hero-text">
            <span class="section-subtitle">Chromatic Family Salon • Dum Dum</span>
            <h1>Crafting Your <br><span class="accent" id="rotatingWord">Signature</span> <br>Look</h1>
            <p>Where luxury meets artistry. Experience bespoke hair care, refined styling, and personalized beauty treatments crafted exclusively for you and your family.</p>
            <div class="hero-cta">
                <a href="https://wa.me/919163499293?text=Hi%20Chromatic%20Family%20Salon!%20%F0%9F%91%8B%20I'd%20like%20to%20book%20an%20appointment.%20Can%20you%20help%20me%20with%20available%20slots%3F" class="btn-premium btn-filled book-trigger" target="_blank">Book Appointment</a>
                <a href="#services" class="btn-premium">Explore Services</a>
            </div>
        </div>
        <div class="hero-image-wrapper">
            <div class="hero-image"></div>
        </div>
        <div class="scroll-indicator">Scroll</div>
    </section>

    <!-- Philosophy / About -->
    <section id="philosophy">
        <div class="container">
            <div class="philosophy-grid">
                <div class="philosophy-image reveal"></div>
                <div class="philosophy-text reveal">
                    <span class="section-subtitle">Our Philosophy</span>
                    <h2 class="section-title">Where Elegance Meets Expertise</h2>
                    <p>At Chromatic Family Salon, we believe that a visit to the salon should be an escape—a moment of pure luxury and rejuvenation. Nestled in the heart of Dum Dum, Kolkata, we have curated an environment where world-class artistry meets warm, family-oriented hospitality.</p>
                    <p>Our master stylists and beauty experts are dedicated to understanding your unique features, ensuring that every cut, color, and treatment is tailored to perfection. From bespoke bridal couture to executive men's grooming, we redefine the standard of salon excellence.</p>
                    <a href="#services" class="btn-premium" style="margin-top: 1rem;">Explore Our Craft</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Services -->
    <section id="services">
        <div class="container text-center">
            <span class="section-subtitle reveal">What We Offer</span>
            <h2 class="section-title reveal">Curated Services</h2>
            <div class="services-grid">
                <div class="service-card reveal">
                    <i class="fas fa-cut"></i>
                    <h3>Bespoke Styling</h3>
                    <p>Precision haircuts, advanced coloring techniques, and bespoke styling tailored to your unique persona.</p>
                </div>
                <div class="service-card reveal">
                    <i class="fas fa-spa"></i>
                    <h3>Luxury Hair Spa</h3>
                    <p>Rejuvenating scalp treatments, deep conditioning rituals, and advanced keratin therapies for ultimate hair health.</p>
                </div>
                <div class="service-card reveal">
                    <i class="fas fa-gem"></i>
                    <h3>Bridal Couture</h3>
                    <p>Exquisite bridal makeup, intricate hairstyling, and pre-bridal skincare packages to make your day flawless.</p>
                </div>
                <div class="service-card reveal">
                    <i class="fas fa-user-tie"></i>
                    <h3>Executive Grooming</h3>
                    <p>Classic and contemporary men's grooming, including hot towel shaves, beard sculpting, and premium facials.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery -->
    <section id="gallery">
        <div class="container text-center">
            <span class="section-subtitle reveal">Our Portfolio</span>
            <h2 class="section-title reveal">The Chromatic Gallery</h2>
            <div class="gallery-grid">
                <div class="gallery-item reveal"><img src="https://images.unsplash.com/photo-1562322140-8baeececf3df?auto=format&fit=crop&w=800&q=80" alt="Hair Styling"></div>
                <div class="gallery-item reveal"><img src="https://images.unsplash.com/photo-1595476108010-b4d1f102b1b1?auto=format&fit=crop&w=800&q=80" alt="Salon Interior"></div>
                <div class="gallery-item reveal"><img src="https://images.unsplash.com/photo-1560066984-138dadb4c035?auto=format&fit=crop&w=800&q=80" alt="Hair Coloring"></div>
                <div class="gallery-item reveal"><img src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?auto=format&fit=crop&w=800&q=80" alt="Makeup"></div>
                <div class="gallery-item reveal"><img src="https://images.unsplash.com/photo-1633681926022-84c23e8cb2d6?auto=format&fit=crop&w=800&q=80" alt="Salon Tools"></div>
            </div>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact">
        <div class="container">
            <div class="text-center">
                <span class="section-subtitle reveal">Get In Touch</span>
                <h2 class="section-title reveal">Visit Our Studio</h2>
            </div>
            <div class="contact-grid">
                <div class="contact-details reveal">
                    <div class="contact-item">
                        <h4>Location</h4>
                        <p>Dum Dum, Kolkata,<br>West Bengal, India</p>
                    </div>
                    <div class="contact-item">
                        <h4>Reservations</h4>
                        <a href="tel:9163499293">+91 91634 99293</a>
                    </div>
                    <div class="contact-item">
                        <h4>Operating Hours</h4>
                        <p>Monday – Sunday<br>10:00 AM – 9:00 PM</p>
                    </div>
                    <div class="contact-item">
                        <h4>Follow Our Journey</h4>
                        <a href="#">@chromaticfamilysalon</a>
                    </div>
                    <a href="https://wa.me/919163499293?text=Hi%20Chromatic%20Family%20Salon!%20%F0%9F%91%8B%20I'd%20like%20to%20book%20an%20appointment.%20Can%20you%20help%20me%20with%20available%20slots%3F" class="btn-premium btn-filled book-trigger" target="_blank" style="align-self: flex-start; margin-top: 1rem;">
                        <i class="fab fa-whatsapp"></i> &nbsp; Book via WhatsApp
                    </a>
                </div>
                <div class="map-container reveal">
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2948.541!2d88.4145!3d22.6192!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjLCsDM3JzA5LjEiTiA4OMKwMjQnNTIuMiJF!5e0!3m2!1sen!2sin!4v1620000000000!5m2!1sen!2sin" 
                        allowfullscreen="" 
                        loading="lazy">
                    </iframe>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-logo">Chromatic <span>Family</span></div>
        <div class="social-links">
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="https://wa.me/919163499293?text=Hi%20Chromatic%20Family%20Salon!%20%F0%9F%91%8B%20I%20visited%20your%20website%20and%20would%20love%20to%20know%20more%20about%20your%20services." target="_blank"><i class="fab fa-whatsapp"></i></a>
        </div>
        <p>&copy; 2026 Chromatic Family Salon. Dum Dum, Kolkata. All Rights Reserved.</p>
    </footer>

    <!-- FLOATING WHATSAPP BUTTON -->
    <a href="https://wa.me/919163499293?text=Hi%20Chromatic%20Family%20Salon!%20%F0%9F%91%8B%20I%20visited%20your%20website%20and%20would%20love%20to%20know%20more%20about%20your%20services." 
       class="whatsapp-float" 
       target="_blank" 
       aria-label="Chat on WhatsApp">
        <i class="fab fa-whatsapp"></i>
        <span class="tooltip">Chat with us</span>
    </a>

    <!-- JavaScript -->
    <script>
        // Navbar Scroll Effect
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });

        // Mobile Menu Toggle
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');
        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });

        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => navLinks.classList.remove('active'));
        });

        // Scroll Reveal Animation
        const reveals = document.querySelectorAll('.reveal');
        const revealOnScroll = () => {
            reveals.forEach(element => {
                const windowHeight = window.innerHeight;
                const elementTop = element.getBoundingClientRect().top;
                const revealPoint = 100;

                if (elementTop < windowHeight - revealPoint) {
                    element.classList.add('active');
                }
            });
        };

        window.addEventListener('scroll', revealOnScroll);
        window.addEventListener('load', revealOnScroll);

        // HERO ROTATING WORD ANIMATION
        const words = ['Signature', 'Perfect', 'Unique', 'Stunning', 'Timeless'];
        let wordIndex = 0;
        const rotatingWord = document.getElementById('rotatingWord');

        setInterval(() => {
            rotatingWord.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            rotatingWord.style.opacity = '0';
            rotatingWord.style.transform = 'translateY(-20px)';
            
            setTimeout(() => {
                wordIndex = (wordIndex + 1) % words.length;
                rotatingWord.textContent = words[wordIndex];
                rotatingWord.style.transform = 'translateY(20px)';
                
                setTimeout(() => {
                    rotatingWord.style.opacity = '1';
                    rotatingWord.style.transform = 'translateY(0)';
                }, 50);
            }, 500);
        }, 2500);
    </script>
</body>
</html>


  