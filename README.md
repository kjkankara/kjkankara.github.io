<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pokoje Gościnne Ćwików</title>
  <link rel="stylesheet" href="style.css">
  <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY&callback=initMap" async defer></script>
</head>
<body>
  <header>
    <div class="container">
      <h1>Pokoje Gościnne Ćwików</h1>
      <nav>
        <ul>
          <li><a href="#home">Strona Główna</a></li>
          <li><a href="#oferta">Oferta</a></li>
          <li><a href="#galeria">Galeria</a></li>
          <li><a href="#kontakt">Kontakt</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <section id="home" class="hero">
    <div class="container">
      <h2>Odkryj urok Ćwikowa</h2>
      <p>Ciesz się relaksem w otoczeniu pięknej natury i korzystaj z atrakcji rekreacyjnych, takich jak jazda konna.</p>
    </div>
  </section>

  <section id="oferta" class="section">
    <div class="container">
      <h2>Nasza Oferta</h2>
      <p>Oferujemy 4 komfortowe pokoje: 3 dwuosobowe i 1 jednoosobowy, każdy z prywatną łazienką, a także dostęp do aneksu kuchennego.</p>
      <ul>
        <li>3 pokoje dwuosobowe</li>
        <li>1 pokój jednoosobowy z możliwością dostawienia dodatkowego łóżka</li>
        <li>Aneks kuchenny w części wspólnej</li>
      </ul>
      <h3>Dodatkowe Usługi</h3>
      <p>Oferujemy szkolenia z jazdy konnej, przejażdżki bryczką oraz transport koni.</p>
    </div>
  </section>

  <section id="galeria" class="section">
    <div class="container">
      <h2>Galeria</h2>
      <div class="gallery">
        <img src="images/pokoj1.jpg" alt="Pokój 1">
        <img src="images/pokoj2.jpg" alt="Pokój 2">
        <img src="images/pokoj3.jpg" alt="Pokój 3">
        <img src="images/natura.jpg" alt="Natura Ćwikowa">
      </div>
    </div>
  </section>

  <section id="kontakt" class="section">
    <div class="container">
      <h2>Skontaktuj się z nami!</h2>
      <p>Chętnie odpowiemy na wszelkie pytania dotyczące naszej oferty i dostępności pokoi.</p>
      <p>Telefon: 999 999 999</p>
      <p>Adres: Ćwików 196, 33-210 Ćwików</p>

      <div id="map"></div>
    </div>
  </section>

  <footer>
    <div class="container">
      <p>&copy; 2025 Pokoje Gościnne Ćwików</p>
    </div>
  </footer>

  <script>
    function initMap() {
      var myLatLng = {lat: 49.8531, lng: 20.0434}; // Współrzędne dla Ćwikowa
      var map = new google.maps.Map(document.getElementById('map'), {
        zoom: 15,
        center: myLatLng
      });
      var marker = new google.maps.Marker({
        position: myLatLng,
        map: map,
        title: 'Ćwików 196'
      });
    }
  </script>
</body>
</html>
