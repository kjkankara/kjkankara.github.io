<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pokoje Gościnne Ćwików | Komfort w sercu natury</title>
    <style>
        :root {
            --primary-color: #4e7a51;
            --secondary-color: #f5b642;
            --accent-color: #9c4a31;
            --light-color: #f8f5e4;
            --dark-color: #2e3a23;
            --shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light-color);
            color: var(--dark-color);
            line-height: 1.6;
        }
        
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: var(--shadow);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
        }
        
        .logo-icon {
            margin-right: 10px;
            font-size: 2rem;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 2rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
            font-size: 1.1rem;
        }
        
        nav ul li a:hover {
            color: var(--secondary-color);
        }
        
        #mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        .hero {
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/api/placeholder/1200/600');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 8rem 2rem;
            margin-bottom: 3rem;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        
        .hero p {
            font-size: 1.3rem;
            max-width: 800px;
            margin: 0 auto;
            margin-bottom: 2rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--secondary-color);
            color: var(--dark-color);
            padding: 1rem 2rem;
            font-size: 1.1rem;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: var(--shadow);
        }
        
        .cta-button:hover {
            background-color: #e4a52f;
            transform: translateY(-3px);
        }
        
        section {
            padding: 4rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            color: var(--primary-color);
            font-size: 2.5rem;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 1rem auto;
        }
        
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-top: 3rem;
        }
        
        .feature {
            flex: 0 0 calc(33.333% - 2rem);
            margin-bottom: 3rem;
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: var(--shadow);
            transition: transform 0.3s ease;
            text-align: center;
        }
        
        .feature:hover {
            transform: translateY(-10px);
        }
        
        .feature i {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 1.5rem;
        }
        
        .feature h3 {
            margin-bottom: 1rem;
            color: var(--dark-color);
        }
        
        .about {
            background-color: var(--primary-color);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }
        
        .about-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .about h2 {
            color: white;
        }
        
        .about h2::after {
            background-color: white;
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-top: 2rem;
        }
        
        .contact-item {
            flex: 0 0 calc(33.333% - 2rem);
            margin-bottom: 2rem;
            text-align: center;
            padding: 2rem;
            background-color: white;
            border-radius: 10px;
            box-shadow: var(--shadow);
        }
        
        .contact-item i {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        
        .contact-item h3 {
            margin-bottom: 1rem;
        }
        
        .map-container {
            height: 400px;
            margin-top: 3rem;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }
        
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }
        
        .footer-logo {
            font-size: 1.5rem;
            font-weight: bold;
        }
        
        .footer-links {
            display: flex;
            list-style: none;
        }
        
        .footer-links li {
            margin: 0 1rem;
        }
        
        .footer-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-links a:hover {
            color: var(--secondary-color);
        }
        
        .footer-bottom {
            margin-top: 2rem;
            padding-top: 1rem;
            border-top: 1px solid rgba(255,255,255,0.1);
        }
        
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 3rem;
        }
        
        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            box-shadow: var(--shadow);
            height: 250px;
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        
        .gallery-item .overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0,0,0,0.7));
            padding: 1rem;
            color: white;
            transition: opacity 0.3s ease;
            opacity: 0;
        }
        
        .gallery-item:hover .overlay {
            opacity: 1;
        }
        
        .room-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }
        
        .room-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: transform 0.3s ease;
        }
        
        .room-card:hover {
            transform: translateY(-10px);
        }
        
        .room-img {
            height: 200px;
            overflow: hidden;
        }
        
        .room-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .room-card:hover .room-img img {
            transform: scale(1.05);
        }
        
        .room-details {
            padding: 1.5rem;
        }
        
        .room-details h3 {
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }
        
        .room-features {
            display: flex;
            margin: 1rem 0;
            flex-wrap: wrap;
        }
        
        .room-feature {
            display: flex;
            align-items: center;
            margin-right: 1rem;
            margin-bottom: 0.5rem;
        }
        
        .room-feature i {
            color: var(--primary-color);
            margin-right: 0.5rem;
        }
        
        .room-price {
            font-size: 1.3rem;
            color: var(--accent-color);
            font-weight: bold;
            margin: 1rem 0;
        }
        
        .book-btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 0.8rem 1.5rem;
            text-decoration: none;
            border-radius: 5px;
            transition: all 0.3s ease;
            font-weight: 600;
        }
        
        .book-btn:hover {
            background-color: var(--dark-color);
        }
        
        .testimonials {
            background-color: var(--light-color);
            padding: 4rem 0;
        }
        
        .testimonials-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        
        .testimonial {
            flex: 0 0 calc(33.333% - 2rem);
            margin-bottom: 2rem;
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: var(--shadow);
        }
        
        .testimonial-text {
            margin-bottom: 1.5rem;
            font-style: italic;
            position: relative;
        }
        
        .testimonial-text::before {
            content: '"';
            font-size: 4rem;
            color: rgba(78, 122, 81, 0.2);
            position: absolute;
            top: -1.5rem;
            left: -1rem;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 1rem;
            object-fit: cover;
        }
        
        .author-info h4 {
            color: var(--dark-color);
        }
        
        .author-info p {
            color: var(--primary-color);
            font-size: 0.9rem;
        }
        
        .activities {
            margin-top: 4rem;
        }
        
        .activities-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .activity-card {
            position: relative;
            height: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }
        
        .activity-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .activity-card:hover img {
            transform: scale(1.05);
        }
        
        .activity-info {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            padding: 1.5rem;
            background: linear-gradient(transparent, rgba(0,0,0,0.8));
            color: white;
        }
        
        .activity-info h3 {
            margin-bottom: 0.5rem;
        }
        
        .activity-info p {
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }
        
        .activity-info a {
            display: inline-block;
            padding: 0.5rem 1rem;
            background-color: var(--secondary-color);
            color: var(--dark-color);
            text-decoration: none;
            border-radius: 5px;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .activity-info a:hover {
            background-color: white;
        }
        
        form {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: var(--shadow);
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--dark-color);
        }
        
        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        .form-group textarea {
            height: 150px;
        }
        
        .submit-btn {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 1rem 2rem;
            font-size: 1.1rem;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .submit-btn:hover {
            background-color: var(--dark-color);
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 0.5rem 0;
            }
            
            .feature, 
            .contact-item,
            .testimonial {
                flex: 0 0 100%;
            }
            
            .footer-content {
                flex-direction: column;
            }
            
            .footer-logo,
            .footer-links {
                margin-bottom: 1rem;
            }
            
            #mobile-menu-btn {
                display: block;
                position: absolute;
                top: 1rem;
                right: 2rem;
            }
            
            #main-nav {
                display: none;
                width: 100%;
            }
            
            #main-nav.active {
                display: block;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <a href="index.html" class="logo">
                    <i class="fas fa-home logo-icon"></i>
                    Pokoje Gościnne Ćwików
                </a>
                <button id="mobile-menu-btn">
                    <i class="fas fa-bars"></i>
                </button>
                <nav id="main-nav">
                    <ul>
                        <li><a href="#" class="active">Strona Główna</a></li>
                        <li><a href="#rooms">Oferta</a></li>
                        <li><a href="#gallery">Galeria</a></li>
                        <li><a href="#about">O Nas</a></li>
                        <li><a href="#contact">Kontakt</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Odkryj Magię Ćwikowa</h1>
            <p>Komfortowe pokoje gościnne w sercu malowniczej natury Małopolski. Relaks, cisza i piękne widoki czekają na Ciebie.</p>
            <a href="#contact" class="cta-button">Zarezerwuj Pobyt</a>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features">
        <div class="container">
            <h2 class="section-title">Dlaczego My?</h2>
            <div class="features">
                <div class="feature">
                    <i class="fas fa-bed"></i>
                    <h3>Komfortowe Pokoje</h3>
                    <p>4 wygodne pokoje z prywatnymi łazienkami, zapewniające intymność i wypoczynek po dniu pełnym wrażeń.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-tree"></i>
                    <h3>Piękna Lokalizacja</h3>
                    <p>Położenie w malowniczej okolicy z wieloma terenami zielonymi, idealnymi do rekreacji i relaksu.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-horse"></i>
                    <h3>Jazda Konna</h3>
                    <p>Oferujemy szkolenia z jazdy konnej, przejażdżki bryczką oraz organizację wycieczek konnych.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Rooms Section -->
    <section id="rooms">
        <div class="container">
            <h2 class="section-title">Nasza Oferta</h2>
            <p style="text-align: center; max-width: 800px; margin: 0 auto 3rem auto;">Oferujemy 4 komfortowe pokoje: 3 dwuosobowe i 1 jednoosobowy z możliwością dostawienia dodatkowego łóżka. Każdy pokój posiada prywatną łazienkę oraz dostęp do wspólnego aneksu kuchennego.</p>
            
            <div class="room-list">
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Pokój Dwuosobowy Standard">
                    </div>
                    <div class="room-details">
                        <h3>Pokój Dwuosobowy Standard</h3>
                        <p>Przytulny pokój z dużym łóżkiem, prywatną łazienką i widokiem na ogród.</p>
                        <div class="room-features">
                            <div class="room-feature">
                                <i class="fas fa-wifi"></i>
                                <span>Wi-Fi</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-shower"></i>
                                <span>Prywatna łazienka</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-tv"></i>
                                <span>TV</span>
                            </div>
                        </div>
                        <div class="room-price">
                            od 200 PLN / noc
                        </div>
                        <a href="#contact" class="book-btn">Zarezerwuj</a>
                    </div>
                </div>
                
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Pokój Dwuosobowy Deluxe">
                    </div>
                    <div class="room-details">
                        <h3>Pokój Dwuosobowy Deluxe</h3>
                        <p>Przestronny pokój z dużym łóżkiem, prywatną łazienką i widokiem na okolicę.</p>
                        <div class="room-features">
                            <div class="room-feature">
                                <i class="fas fa-wifi"></i>
                                <span>Wi-Fi</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-shower"></i>
                                <span>Prywatna łazienka</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-tv"></i>
                                <span>TV</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-couch"></i>
                                <span>Strefa wypoczynku</span>
                            </div>
                        </div>
                        <div class="room-price">
                            od 250 PLN / noc
                        </div>
                        <a href="#contact" class="book-btn">Zarezerwuj</a>
                    </div>
                </div>
                
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Pokój Jednoosobowy">
                    </div>
                    <div class="room-details">
                        <h3>Pokój Jednoosobowy</h3>
                        <p>Przytulny pokój dla jednej osoby z możliwością dostawienia łóżka i prywatną łazienką.</p>
                        <div class="room-features">
                            <div class="room-feature">
                                <i class="fas fa-wifi"></i>
                                <span>Wi-Fi</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-shower"></i>
                                <span>Prywatna łazienka</span>
                            </div>
                            <div class="room-feature">
                                <i class="fas fa-tv"></i>
                                <span>TV</span>
                            </div>
                        </div>
                        <div class="room-price">
                            od 150 PLN / noc
                        </div>
                        <a href="#contact" class="book-btn">Zarezerwuj</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Activities Section -->
    <section id="activities">
        <div class="container">
            <h2 class="section-title">Atrakcje</h2>
            <p style="text-align: center; max-width: 800px; margin: 0 auto 3rem auto;">Ćwików i okolice oferują wiele atrakcji dla miłośników aktywnego wypoczynku oraz osób poszukujących wyciszenia w otoczeniu natury.</p>
            
            <div class="activities-grid">
                <div class="activity-card">
                    <img src="/api/placeholder/400/300" alt="Jazda konna">
                    <div class="activity-info">
                        <h3>Jazda Konna</h3>
                        <p>Oferujemy profesjonalne szkolenia z jazdy konnej zarówno dla początkujących, jak i zaawansowanych.</p>
                        <a href="#contact">Dowiedz się więcej</a>
                    </div>
                </div>
                
                <div class="activity-card">
                    <img src="/api/placeholder/400/300" alt="Przejażdżki bryczką">
                    <div class="activity-info">
                        <h3>Przejażdżki Bryczką</h3>
                        <p>Poznaj uroki okolicy podczas romantycznej przejażdżki tradycyjną bryczką.</p>
                        <a href="#contact">Dowiedz się więcej</a>
                    </div>
                </div>
                
                <div class="activity-card">
                    <img src="/api/placeholder/400/300" alt="Ogniska">
                    <div class="activity-info">
                        <h3>Ogniska</h3>
                        <p>Zorganizuj ognisko w otoczeniu przyrody i ciesz się wspólnym czasem z bliskimi.</p>
                        <a href="#contact">Dowiedz się więcej</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery">
        <div class="container">
            <h2 class="section-title">Galeria</h2>
            
            <div class="gallery">
                <div class="gallery-item">
                    <img src="/api/placeholder/400/300" alt="Pokój gościnny">
                    <div class="overlay">
                        <h3>Pokój Dwuosobowy Deluxe</h3>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="/api/placeholder/400/300" alt="Łazienka">
                    <div class="overlay">
                        <h3>Nowoczesna łazienka</h3>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="/api/placeholder/400/300" alt="Aneks kuchenny">
                    <div class="overlay">
                        <h3>Aneks kuchenny</h3>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="/api/placeholder/400/300" alt="Widok na okolicę">
                    <div class="overlay">
                        <h3>Malownicza okolica</h3>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="/api/placeholder/400/300" alt="Jazda konna">
                    <div class="overlay">
                        <h3>Jazda konna</h3>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="/api/placeholder/400/300" alt="Przejażdżka bryczką">
                    <div class="overlay">
                        <h3>Przejażdżka bryczką</h3>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials">
        <div class="container">
            <h2 class="section-title">Opinie Gości</h2>
            
            <div class="testimonials-container">
                <div class="testimonial">
                    <div class="testimonial-text">
                        <p>Przepiękne miejsce z dala od zgiełku miasta. Pokoje czyste i przytulne, a gospodarze niezwykle gościnni. Jazda konna była dodatkową atrakcją, którą szczególnie polecam.</p>
                    </div>
                    <div class="testimonial-author">
                        <img src="/api/placeholder/50/50" alt="Anna K.">
                        <div class="author-info">
                            <h4>Anna K.</h4>
                            <p>Kraków</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-text">
                        <p>Świetne miejsce na weekend z rodziną. Dzieci były zachwycone przejażdżką bryczką, a my mogliśmy odpocząć w pięknym otoczeniu natury. Na pewno wrócimy!</p>
                    </div>
                    <div class="testimonial-author">
                        <img src="/api/placeholder/50/50" alt="Michał T.">
                        <div class="author-info">
                            <h4>Michał T.</h4>
                            <p>Katowice</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-text">
                        <p>Idealne miejsce dla miłośników koni i natury. Pokoje komfortowe, a
