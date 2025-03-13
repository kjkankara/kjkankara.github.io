<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pokoje Gościnne Ćwików</title>
    <link rel="stylesheet" href="styles.css">
    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" async defer></script>
</head>
<body>
    <header class="hero">
        <div class="hero-content">
            <h1>Pokoje Gościnne Ćwików</h1>
            <p>Odkryj urok Ćwikowa – komfortowe pokoje w malowniczej okolicy.</p>
            <a href="#offer" class="btn">Sprawdź ofertę</a>
        </div>
    </header>

    <nav class="navbar">
        <ul>
            <li><a href="#home">Strona Główna</a></li>
            <li><a href="#offer">Oferta</a></li>
            <li><a href="#gallery">Galeria</a></li>
            <li><a href="#contact">Kontakt</a></li>
        </ul>
    </nav>

    <section id="home" class="section">
        <h2>Witamy w Ćwikowie!</h2>
        <p>Ćwików to miejsce, gdzie możesz odpocząć w otoczeniu natury i skorzystać z atrakcji takich jak jazda konna czy organizacja ognisk. Nasze pokoje są idealne dla osób szukających komfortu i relaksu.</p>
    </section>

    <section id="offer" class="section">
        <h2>Nasza Oferta</h2>
        <div class="offer-grid">
            <div class="offer-item">
                <h3>Komfortowe Pokoje</h3>
                <p>4 pokoje: 3 dwuosobowe i 1 jednoosobowy z możliwością dostawienia dodatkowego łóżka. Każdy pokój posiada prywatną łazienkę.</p>
            </div>
            <div class="offer-item">
                <h3>Piękna Lokalizacja</h3>
                <p>Malownicze tereny zielone idealne do rekreacji, jazdy konnej oraz organizacji ognisk.</p>
            </div>
            <div class="offer-item">
                <h3>Dodatkowe Usługi</h3>
                <p>Szkolenia z jazdy konnej, przejażdżki bryczką oraz transport koni – idealne dla miłośników zwierząt.</p>
            </div>
        </div>
    </section>

    <section id="gallery" class="section">
        <h2>Galeria</h2>
        <div class="gallery-grid">
            <!-- Replace these with actual image paths -->
            <img src="room1.jpg" alt="Pokój 1">
            <img src="room2.jpg" alt="Pokój 2">
            <img src="room3.jpg" alt="Pokój 3">
        </div>
    </section>

    <section id="contact" class="section contact-section">
        <h2>Skontaktujmy się!</h2>
        <p>Zapraszamy do kontaktu! Chętnie odpowiemy na wszelkie pytania dotyczące naszej oferty.</p>
        <p><strong>Telefon:</strong> 999 999 999</p>
        <p><strong>Adres:</strong> Ćwików 196, Ćwików, 33-210</p>

        <!-- Map -->
        <div id="map"></div>

        <script>
            function initMap() {
                var location = {lat: 49.7339, lng: 19.5798}; // Replace with actual coordinates
                var map = new google.maps.Map(document.getElementById('map'), {
                    zoom: 15,
                    center: location
                });
                var marker = new google.maps.Marker({
                    position: location,
                    map: map
                });
            }
        </script>
    </section>

    <footer class="footer">
        &copy; 2025 Pokoje Gościnne Ćwików. Wszelkie prawa zastrzeżone.
    </footer>

</body>
</html>

