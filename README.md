<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pokoje do wynajęcia | Ćwików, Oleśno</title>
    <style>
        :root {
            --primary-color: #3a5a40;
            --secondary-color: #588157;
            --accent-color: #a3b18a;
            --light-color: #dad7cd;
            --dark-color: #344e41;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light-color);
            color: #333;
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('/api/placeholder/1200/600') center/cover no-repeat;
            color: white;
            text-align: center;
            padding: 3rem 1rem;
            min-height: 50vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        section {
            padding: 4rem 0;
        }
        
        section:nth-child(even) {
            background-color: white;
        }
        
        h1, h2, h3 {
            color: var(--dark-color);
            margin-bottom: 1rem;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: white;
        }
        
        h2 {
            font-size: 2rem;
            text-align: center;
            position: relative;
            margin-bottom: 2.5rem;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: var(--secondary-color);
        }
        
        p {
            margin-bottom: 1.5rem;
        }
        
        .intro {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            text-align: center;
        }
        
        /* Rooms */
        .rooms {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .room-card {
            background-color: white;
            border-radius: 5px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
            overflow: hidden;
        }
        
        .room-img {
            height: 200px;
            overflow: hidden;
        }
        
        .room-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .room-info {
            padding: 1.5rem;
        }
        
        .room-info h3 {
            margin-bottom: 0.5rem;
        }
        
        /* Services */
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            text-align: center;
            padding: 2rem;
            border-radius: 5px;
            background-color: white;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
        }
        
        .service-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--secondary-color);
        }
        
        /* Gallery */
        .gallery-section {
            margin-bottom: 3rem;
        }
        
        .gallery-title {
            margin-bottom: 1.5rem;
            text-align: center;
            color: var(--dark-color);
        }
        
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            overflow: hidden;
            border-radius: 5px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
            height: 250px;
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        
        /* Map */
        .map-container {
            height: 400px;
            border-radius: 5px;
            overflow: hidden;
            margin-top: 2rem;
        }
        
        /* Contact */
        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 1.5rem;
        }
        
        .contact-icon {
            width: 40px;
            height: 40px;
            background-color: var(--secondary-color);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.8rem;
            }
            
            .gallery-item {
                height: 200px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Pokoje do wynajęcia w Ćwikowie</h1>
        <p>Odkryj piękno natury i komfortowy wypoczynek w malowniczej okolicy Oleśna</p>
    </header>
    
    <section id="about">
        <div class="container">
            <h2>O nas</h2>
            <p class="intro">
                Witamy w naszym obiekcie położonym w malowniczej miejscowości Ćwików w województwie małopolskim. 
                Oferujemy komfortowy wypoczynek w otoczeniu pięknej przyrody, z dala od miejskiego zgiełku.
            </p>
            
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-top: 2rem;">
                <div>
                    <h3>Nasza oferta</h3>
                    <p>Oferujemy 4 komfortowe pokoje: 3 dwuosobowe i 1 jednoosobowy z możliwością dostawienia dodatkowego łóżka. Każdy pokój posiada prywatną łazienkę, co zapewnia wygodę i intymność dla gości.</p>
                    <p>W części wspólnej dostępny jest aneks kuchenny do dyspozycji wszystkich gości, wyposażony we wszystko, co potrzebne do przygotowania posiłków.</p>
                </div>
                
                <div>
                    <h3>Dla miłośników koni</h3>
                    <p>Nasza oferta skierowana jest szczególnie do miłośników koni. Oferujemy lekcje jazdy konnej dla początkujących i zaawansowanych, przejażdżki w terenie, a także możliwość transportu koni dla gości, którzy chcą przyjechać ze swoimi zwierzętami.</p>
                    <p>Nasz obiekt to miejsce stworzone z miłości do gościnności oraz pięknej natury.</p>
                </div>
                
                <div>
                    <h3>Okolica</h3>
                    <p>Lokalizacja Ćwików znajduje się w malowniczej okolicy z wieloma terenami zielonymi, idealnymi do rekreacji, jazdy konnej oraz pieszych wędrówek. To doskonałe miejsce dla osób szukających odpoczynku od miejskiego zgiełku.</p>
                    <p>Nasza misja to stworzenie przyjaznej przestrzeni, w której każdy może odpocząć i cieszyć się otaczającą przyrodą.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section id="rooms">
        <div class="container">
            <h2>Nasze pokoje</h2>
            <p class="intro">
                Obiekt oferuje 4 komfortowe pokoje, każdy z prywatną łazienką. Wszystkie pokoje są czyste, przytulne i dobrze wyposażone, 
                aby zapewnić naszym gościom komfortowy pobyt.
            </p>
            
            <div class="rooms">
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Pokoje">
                    </div>
                    <div class="room-info">
                        <h3>Pokoje dwuosobowe</h3>
                        <p>Oferujemy trzy przestronne pokoje dwuosobowe, idealne dla par lub osób podróżujących we dwoje. Każdy pokój wyposażony jest w wygodne łóżka, szafę oraz prywatną łazienkę z prysznicem.</p>
                    </div>
                </div>
                
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Pokój jednoosobowy">
                    </div>
                    <div class="room-info">
                        <h3>Pokój jednoosobowy</h3>
                        <p>Dla osób podróżujących samotnie przygotowaliśmy przytulny pokój jednoosobowy z możliwością dostawienia dodatkowego łóżka. Pokój posiada prywatną łazienkę, biurko oraz wszystko, co potrzebne do komfortowego pobytu.</p>
                    </div>
                </div>
                
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Łazienka">
                    </div>
                    <div class="room-info">
                        <h3>Prywatne łazienki</h3>
                        <p>Każdy pokój posiada nowoczesną, prywatną łazienkę z prysznicem, umywalką i toaletą. Zapewniamy ręczniki i podstawowe kosmetyki dla naszych gości.</p>
                    </div>
                </div>
                
                <div class="room-card">
                    <div class="room-img">
                        <img src="/api/placeholder/400/300" alt="Aneks kuchenny">
                    </div>
                    <div class="room-info">
                        <h3>Wspólny aneks kuchenny</h3>
                        <p>Do dyspozycji wszystkich gości jest w pełni wyposażony aneks kuchenny, gdzie można przygotować i spożyć posiłki. Znajduje się tam lodówka, kuchenka, czajnik, naczynia oraz sztućce.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="services">
        <div class="container">
            <h2>Nasze usługi</h2>
            <p class="intro">
                Oprócz komfortowego zakwaterowania, oferujemy szereg dodatkowych atrakcji związanych głównie z jazdą konną.
            </p>
            
            <div class="services">
                <div class="service-card">
                    <div class="service-icon">🐎</div>
                    <h3>Jazda konna</h3>
                    <p>Oferujemy lekcje jazdy konnej dla początkujących oraz zaawansowanych pod okiem doświadczonych instruktorów. Doskonała okazja dla miłośników koni.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">🌿</div>
                    <h3>Tereny zielone</h3>
                    <p>Nasz obiekt położony jest w otoczeniu pięknych terenów zielonych, idealnych do rekreacji, spacerów i aktywnego wypoczynku na świeżym powietrzu.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">🚶‍♂️</div>
                    <h3>Przejażdżki bryczką</h3>
                    <p>Proponujemy przejażdżki bryczką po malowniczej okolicy, które pozwolą podziwiać piękne krajobrazy i spędzić czas w nietypowy sposób.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">🐴</div>
                    <h3>Transport koni</h3>
                    <p>Oferujemy usługi transportu koni dla gości, którzy chcą przyjechać ze swoimi końmi i korzystać z okolicznych terenów do jazdy.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">🍳</div>
                    <h3>Aneks kuchenny</h3>
                    <p>Do dyspozycji gości udostępniamy w pełni wyposażony aneks kuchenny w części wspólnej, gdzie można przygotować własne posiłki.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">🔥</div>
                    <h3>Możliwość organizacji ogniska</h3>
                    <p>Na życzenie gości możemy zorganizować ognisko, gdzie można spędzić wieczór w miłej atmosferze.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section id="gallery">
        <div class="container">
            <h2>Galeria</h2>
            
            <div class="gallery-section">
                <h3 class="gallery-title">Pokoje i wnętrza</h3>
                <div class="gallery">
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Pokój dwuosobowy 1">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Pokój dwuosobowy 2">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Pokój jednoosobowy">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Łazienka">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Aneks kuchenny">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Korytarz">
                    </div>
                </div>
            </div>
            
            <div class="gallery-section">
                <h3 class="gallery-title">Konie i okolica</h3>
                <div class="gallery">
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Koń w stajni">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Jazda konna">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Bryczka">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Okolica - łąki">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Okolica - las">
                    </div>
                    <div class="gallery-item">
                        <img src="/api/placeholder/400/300" alt="Widok z obiektu">
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="location">
        <div class="container">
            <h2>Lokalizacja</h2>
            <p class="intro">
                Nasz obiekt znajduje się w malowniczej miejscowości Ćwików w województwie małopolskim. 
                Dokładny adres: Ćwików 196, 33-210 Oleśno.
            </p>
            
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 2rem;">
                <div>
                    <h3>Jak do nas dojechać?</h3>
                    <div style="margin-top: 1rem;">
                        <h4 style="color: var(--secondary-color);">Samochodem:</h4>
                        <ul style="list-style-position: inside; padding-left: 0; margin-bottom: 1.5rem;">
                            <li>Z Krakowa: ok. 80 km, trasa przez Brzesko i Dąbrowę Tarnowską</li>
                            <li>Z Tarnowa: ok. 30 km, trasa przez Żabno</li>
                            <li>Z Kielc: ok. 120 km, trasa przez Busko-Zdrój i Dąbrowę Tarnowską</li>
                        </ul>
                        
                        <h4 style="color: var(--secondary-color);">Komunikacją publiczną:</h4>
                        <ul style="list-style-position: inside; padding-left: 0;">
                            <li>Najbliższa stacja kolejowa: Dąbrowa Tarnowska (15 km)</li>
                            <li>Autobus do Oleśna z Tarnowa lub Dąbrowy Tarnowskiej</li>
                            <li>Z Oleśna do Ćwikowa: 5 km (możliwy transport po wcześniejszym ustaleniu)</li>
                        </ul>
                    </div>
                </div>
                
                <div>
                    <h3>Co warto zobaczyć w okolicy?</h3>
                    <ul style="list-style-position: inside; padding-left: 0;">
                        <li style="margin-bottom: 0.5rem;"><strong>Zalew w Radłowie</strong> (15 km) - miejsce rekreacji, kąpielisko</li>
                        <li style="margin-bottom: 0.5rem;"><strong>Zamek w Dąbrowie Tarnowskiej</strong> (15 km) - zabytkowa rezydencja</li>
                        <li style="margin-bottom: 0.5rem;"><strong>Tarnów</strong> (30 km) - zabytkowe Stare Miasto, muzea</li>
                        <li style="margin-bottom: 0.5rem;"><strong>Winnice w okolicy Tarnowa</strong> - możliwość zwiedzania i degustacji</li>
                        <li style="margin-bottom: 0.5rem;"><strong>Zalipie</strong> (25 km) - wieś słynąca z malowanych chat</li>
                        <li><strong>Szlaki piesze i rowerowe</strong> - liczne trasy w malowniczej okolicy</li>
                    </ul>
                </div>
            </div>
            
            <div class="map-container">
                <img src="/api/placeholder/1200/400" alt="Mapa z lokalizacją" style="width:100%; height:100%; object-fit:cover;">
            </div>
        </div>
    </section>
    
    <section id="contact">
        <div class="container">
            <h2>Kontakt</h2>
            <div style="max-width: 600px; margin: 0 auto; text-align: center;">
                <p class="intro">
                    Masz pytania? Chcesz dokonać rezerwacji? Zadzwoń do nas!
                </p>
                
                <div class="contact-item" style="justify-content: center;">
                    <div class="contact-icon">📍</div>
                    <div>
                        <h3>Adres</h3>
                        <p>Ćwików 196, 33-210 Oleśno<br>województwo małopolskie</p>
                    </div>
                </div>
                
                <div class="contact-item" style="justify-content: center;">
                    <div class="contact-icon">📞</div>
                    <div>
                        <h3>Telefon</h3>
                        <p style="font-size: 1.2rem; font-weight: bold;">+48 123 456 789</p>
                        <p>Rezerwacji można dokonać wyłącznie telefonicznie</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <p>© 2025 Pokoje do wynajęcia w Ćwikowie | Wszelkie prawa zastrzeżone</p>
        </div>
    </footer>
</body>
</html>
