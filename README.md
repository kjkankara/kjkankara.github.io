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
    <header>
        <h1>Pokoje Gościnne Ćwików</h1>
        <nav>
            <ul>
                <li><a href="#home">Strona Główna</a></li>
                <li><a href="#offer">Oferta</a></li>
                <li><a href="#gallery">Galeria</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Odkryj urok Ćwikowa</h2>
        <p>Gdzie komfortowe pokoje gościnne czekają na Ciebie. Ciesz się relaksem w otoczeniu pięknej natury i korzystaj z atrakcji rekreacyjnych, takich jak jazda konna.</p>
        <h3>Komfortowe Pokoje</h3>
        <p>Obiekt oferuje 4 komfortowe pokoje: 3 dwuosobowe i 1 jednoosobowy z możliwością dostawienia dodatkowego łóżka, każdy z prywatną łazienką, co zapewnia wygodę i intymność dla gości. W części wspólnej dostępny jest aneks kuchenny.</p>
        <h3>Piękna Lokalizacja</h3>
        <p>Ćwików znajduje się w malowniczej okolicy z wieloma terenami zielonymi, idealnymi do rekreacji, jazdy konnej oraz organizacji ognisk.</p>
        <h3>Dodatkowe Usługi</h3>
        <p>Oferujemy szkolenia z jazdy konnej, przejażdżki bryczką oraz transport koni, co stanowi atrakcyjne uzupełnienie oferty dla miłośników koni.</p>
    </section>

    <section id="offer">
        <h2>Nasza Oferta</h2>
        <p>Nasz obiekt to miejsce stworzone z miłości do gościnności oraz pięknej natury. Jako właściciel z wieloletnim doświadczeniem w wynajmie pokoi, pragnę zapewnić naszym gościom komfort i relaks w malowniczym Ćwikowie. Nasza misja to stworzenie przytulnej przestrzeni, w której każdy może odpocząć i cieszyć się otaczającą przyrodą.</p>
    </section>

    <section id="gallery">
        <h2>Galeria</h2>
        <!-- Add images here -->
        <img src="room1.jpg" alt="Pokój 1">
        <img src="room2.jpg" alt="Pokój 2">
        <img src="room3.jpg" alt="Pokój 3">
    </section>

    <section id="contact">
        <h2>Skontaktujmy się!</h2>
        <p>Zapraszamy do kontaktu! Chętnie odpowiemy na wszelkie pytania dotyczące naszej oferty i dostępności pokoi. Czekamy na Was!</p>
        <p>Telefon: 999 999 999</p>
        <p>Adres: Ćwików 196, Ćwików, 33-210</p>

        <!-- Map -->
        <div id="map" style="height: 400px; width: 100%;"></div>

        <script>
            function initMap() {
                var location = {lat: 49.7339, lng: 19.5798}; // Replace with actual coordinates of Ćwików
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

    <footer>
        <p>&copy; 2025 Pokoje Gościnne Ćwików. Wszelkie prawa zastrzeżone.</p>
    </footer>

</body>
</html>

<style>
body {
    font-family: Arial, sans-serif;
    background-color: #f0f8ff;
    color: #333;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    padding: 20px;
}

footer {
    text-align: center;
    padding: 10px;
    background-color: #4CAF50;
    color: white;
}
</style>
