<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Best Places to Visit in India</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css" />
      <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css" integrity="sha512-2SwdPD6INVrV/lHTZbO2nodKhrnDdJK9/kg2XD1r9uGqPo1cUbujc+IYdlYdEErWNu69gVcYgdxlmVmzTWnetw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet">

  <style>
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: linear-gradient(120deg, #f8f8ff 0%, #e0f7fa 100%);
      margin: 0;
      padding: 0;
      min-height: 100vh;
    }
    .navbar {
      display: flex;
      background-color: #e0e0e0cc;
      padding: 10px 10px;
      justify-content: space-evenly;
      align-items: center;
      box-shadow: 0 2px 4px gray;
      color: black;
      overflow: hidden;
      position: sticky;
      top: 0;
      z-index: 10;
      backdrop-filter: blur(4px);
    }
    .navbar a {
      color: #333;
      text-decoration: none;
      margin-left: 15px;
      font-weight: 500;
      transition: background 0.2s, color 0.2s, box-shadow 0.2s;
      padding: 6px 12px;
      border-radius: 3px;
    }
    .navbar a:hover {
      background-color: #b2ebf2;
      color: #00796b;
      box-shadow: 0 2px 8px #b2ebf2;
    }
    .nav-links {
      display: flex;
      align-items: center;
    }
    .menu-btn {
      display: none;
      font-size: 1.5em;
      cursor: pointer;
      margin-right: 10px;
    } .search-box {
      width: 250px;
      padding: 4px;
      border-radius: 20px;
      border: 1px solid pink;
      outline: none;
    }
    .search-btn {
      padding: 8px 8px;
      border: none;
      border-radius: 20px;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
    }
    .search-btn:hover {
      background-color: #45a049;
    }
    .search-box:focus {
      box-shadow: 0 0 8px #b2ebf2;
    }
    .search-btn {
      padding: 7px 12px;
      border: none;
      border-radius: 20px;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
      margin-left: 5px;
      transition: background 0.2s;
    }
    .search-btn:hover {
      background-color: #388e3c;
    }
    .hero {
      margin: 30px auto 20px auto;
      max-width: 700px;
      text-align: center;
      position: relative;
    }
    .animated-bg {
      width: 95vw;
      max-width: 600px;
      height: 280px;
      margin: 0 auto 30px auto;
      border-radius: 18px;
      box-shadow: 0 4px 16px rgba(0,0,0,0.10);
      background-size: cover;
      background-position: center;
      animation: imageSlide 12s infinite;
      transition: background-image 1s;
      position: relative;
      overflow: hidden;
    }
    .animated-bg::after {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: linear-gradient(120deg, rgba(0,0,0,0.18) 0%, rgba(0,0,0,0.08) 100%);
      border-radius: 18px;
      pointer-events: none;
    }
    .hero h1 {
      margin-top: -20px;
      font-size: 2.4em;
      color: #00796b;
      letter-spacing: 1px;
      text-shadow: 0 2px 8px #fff;
    }
    .hero p {
      font-size:1.1em;
      color:#444;
      margin-bottom: 18px;
    }
    .discover-btn {
      background: linear-gradient(90deg, #4CAF50 60%, #00bcd4 100%);
      color: #fff;
      border: none;
      border-radius: 22px;
      padding: 12px 60px;
      font-size: 1.1em;
      font-weight: 600;
      cursor: pointer;
      margin-top: 10px;
      box-shadow: 0 2px 8px #b2ebf2;
      transition: background 0.2s, transform 0.2s;
    }
    .discover-btn:hover {
      background: linear-gradient(90deg, #00bcd4 60%, #4CAF50 100%);
      transform: translateY(-2px) scale(1.03);
    }
    @keyframes imageSlide {
      0%   { background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80'); }
      33%  { background-image: url('https://images.unsplash.com/photo-1465156799763-2c087c332922?auto=format&fit=crop&w=800&q=80'); }
      66%  { background-image: url('https://images.unsplash.com/photo-1500534314209-a25ddb2bd429?auto=format&fit=crop&w=800&q=80'); }
      100% { background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80'); }
    }
    .places-list {
      max-width: 900px;
      margin: 0 auto 40px auto;
      padding: 0 10px;
    }
    .place {
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
      margin-bottom: 28px auto;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      overflow: hidden;
      transition: box-shadow 0.2s, transform 0.2s;
      position: relative;
    }
    .place:hover {
      box-shadow: 0 8px 24px #b2ebf2;
      transform: translateY(-4px) scale(1.01);
      z-index: 2;
    }
    .place img {
      width: 220px;
      height: 150px;
      object-fit: cover;
      border-radius: 12px 0 0 12px;
      flex-shrink: 0;
      transition: filter 0.2s;
      margin: auto;
    }
    .place:hover img {
      filter: brightness(0.92) saturate(1.2);
    }
    .place-content {
      padding: 18px 20px;
      flex: 1;
      min-width: 200px;
    }
    .place-title {
      font-size: 1.3em;
      color: #00796b;
      margin: 0 0 8px 0;
      font-weight: 600;
      letter-spacing: 0.5px;
    }
    .place-desc {
      color: #333;
      margin: 0;
      font-size: 1em;
      line-height: 1.6;
    }
    footer {
      background: #e0e0e0cc;
      padding: 18px 0 10px 0;
      text-align: center;
      color: #00796b;
      font-size: 1.1em;
      letter-spacing: 0.5px;
      border-top: 1px solid #b2ebf2;
      margin-top: 40px;
    }
    .footer-social {
      margin: 10px 0 0 0;
    }
    .footer-social a {
      color: #00796b;
      margin: 0 10px;
      font-size: 1.4em;
      transition: color 0.2s;
      text-decoration: none;
    }
    .footer-social a:hover {
      color: #388e3c;
    }
    @media (max-width: 767px) {
      .navbar {
        flex-direction: column;
        align-items: flex-start;
      }
      .nav-links {
        display: none;
        flex-direction: column;
        width: 100%;
      }
      .nav-links.show {
        display: flex;
      }
      .nav-links a {
        margin: 10px 0 0 0;
        width: 100%;
      }
      .menu-btn {
        display: block;
      }
      .animated-bg {
        height: 180px;
      }
      .hero h1 {
        font-size: 1.3em;
      }
      .place {
        flex-direction: column;
      }
      .place img {
        width: 100%;
        height: 140px;
        border-radius: 12px 12px 0 0;
        margin: 10px auto;
      }
      .place-content {
        padding: 14px 10px;
      }
    }
    @media (max-width: 500px) {
  .hero, .places-list {
    padding-left: 4px;
    padding-right: 4px;
  }
  .discover-btn {
    width: 100%;
    font-size: 1em;
    padding: 12px 0;
  }
}
@media (max-width: 767px) {
  .place {
    flex-direction: column;
  }
  .place img {
    width: 220px;      /* Same as laptop */
    height: 140px;
    border-radius: 12px;
    margin: 12px auto 10px auto; /* Center image */
    display: block;
  }
  .place-content {
    padding: 14px 10px;
  }
}

.price-card {
  background: rgba(173, 216, 230, 0.6);
  border-radius: 15px;
  padding: 20px;
  text-align: center;
  width: 250px;
  margin: 10px;
  transition: 0.3s;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}
.price-card:hover {
  transform: scale(1.05);
  background: rgba(100, 181, 246, 0.7);
}
.btn-primary{
  font-size: 14px;
  text-align: center;
  
}
  </style>
</head>
<body>
  
  <div class="navbar">
    <div class="menu-btn"><i class="fa fa-bars"></i></div>
    <div class="nav-links">
      <a href="website.html">Home</a>
      <a href="about.html">About</a>
      <a href="Privacy.html">Privacy Policy</a>
      <a href="login.html">Login</a>
      <a href="contact.html">Contact</a>
       <a href="Discover more.html">Discover more</a>
    
    </div>
    <form action="https://www.google.com/search" method="get" style="margin:0;">
      <input type="text" name="q" class="search-box" placeholder="Search...">
      <button type="submit" class="search-btn"><i class="fa fa-search"></i></button>
    </form>
    </div>
    
  
  
  

  <div class="hero">
    <div class="animated-bg"></div>
    <h1>Best Places to Visit in India</h1>
    <p>
      Discover the most beautiful and culturally rich destinations across India. From the snowy Himalayas to the sunny beaches of Goa, here are the top places you must visit!
    </p>
    <!-- <button class="discover-btn" onclick="window.scrollTo({top: document.querySelector('.places-list').offsetTop-30, behavior:'smooth'});">
      <i class="fa fa-map-marker-alt"></i> Discover More
    </button> -->
    <a href="Discover more.html" class="discover-btn">
  <i class="fa fa-map-marker-alt"></i> <span style="margin-right: 8px;">Discover More  </span>
</a>
  </div>

  <div class="places-list">
    <div class="place">
        <a href="Discover more.html">
      <img src="https://media.architecturaldigest.com/photos/67acb9b0339bcbaaadeb91b5/1:1/w_4000,h_4000,c_limit/GettyImages-873536102.jpg" alt="Taj Mahal, Agra">
      </a>
      <div class="place-content">
        <div class="place-title">1. Agra (Taj Mahal)</div>
        <p class="place-desc">Home to the iconic Taj Mahal, Agra is a symbol of love and a UNESCO World Heritage Site. The city also boasts Agra Fort and Fatehpur Sikri, making it a must-visit for history lovers.</p>
     <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
    <div class="place">
        <a href="Discover more.html">
      <img src="data:image/jpeg;base64,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" alt="Jaipur, Rajasthan">
     </a>
      <div class="place-content">
        <div class="place-title">2. Jaipur (Rajasthan)</div>
        <p class="place-desc">Known as the Pink City, Jaipur is famous for its royal palaces, vibrant bazaars, and majestic forts like Amber Fort and City Palace. Experience the rich culture and heritage of Rajasthan here.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
    <div class="place">
        <a href="Discover more.html">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRPKttrI6_exgGXfDd6SfoIefbL4trFjZ_nuw&s" alt="Goa">
        </a>
      <div class="place-content">
        <div class="place-title">3. Goa</div>
        <p class="place-desc">Goa is India's party capital, known for its golden beaches, lively nightlife, Portuguese heritage, and delicious seafood. Perfect for relaxation and adventure alike.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
    <div class="place">
        <a href="Discover more.html">
      <img src="https://static2.tripoto.com/media/filter/nl/img/219147/TripDocument/1586429185_kimbalangi.jpeg" alt="Kerala Backwaters">
        </a>
      <div class="place-content">
        <div class="place-title">4. Kerala (Backwaters & Munnar)</div>
       <p class="place-desc">Kerala offers tranquil backwaters, lush tea gardens in Munnar, and beautiful beaches. Enjoy houseboat cruises, wildlife, and Ayurveda in God's Own Country.</p>
        <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
    <div class="place">
        <a href="Discover more.html">
       <img src="data:image/jpeg;base64,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" alt="Varanasi">
        </a>
       <div class="place-content">
        <div class="place-title">5. Varanasi</div>
        <p class="place-desc">One of the world's oldest cities, Varanasi is the spiritual heart of India. Witness the mesmerizing Ganga Aarti and explore ancient temples along the ghats.</p>
     <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
    <div class="place">
        <a href="Discover more.html">
      <img src="https://himachaltourisminfoblog.com/wp-content/uploads/2024/04/Sissu_leh_ladakh-1895x760.jpg" alt="Leh-Ladakh">
        </a>
      <div class="place-content">
        <div class="place-title">6. Leh-Ladakh</div>
        <p class="place-desc">A paradise for adventure seekers, Leh-Ladakh offers breathtaking landscapes, high mountain passes, monasteries, and unique Tibetan culture.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
     <div class="place">
        <a href="Discover more.html">
      <img src="https://himachaltourisminfoblog.com/wp-content/uploads/2024/04/Sissu_leh_ladakh-1895x760.jpg" alt="Leh-Ladakh">
        </a>
      <div class="place-content">
        <div class="place-title">7. Leh-Ladakh</div>
        <p class="place-desc">A paradise for adventure seekers, Leh-Ladakh offers breathtaking landscapes, high mountain passes, monasteries, and unique Tibetan culture.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
     <div class="place">
        <a href="Discover more.html">
      <img src="https://himachaltourisminfoblog.com/wp-content/uploads/2024/04/Sissu_leh_ladakh-1895x760.jpg" alt="Leh-Ladakh">
        </a>
      <div class="place-content">
        <div class="place-title">8. Leh-Ladakh</div>
        <p class="place-desc">A paradise for adventure seekers, Leh-Ladakh offers breathtaking landscapes, high mountain passes, monasteries, and unique Tibetan culture.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
     <div class="place">
        <a href="Discover more.html">
      <img src="https://himachaltourisminfoblog.com/wp-content/uploads/2024/04/Sissu_leh_ladakh-1895x760.jpg" alt="Leh-Ladakh">
        </a>
      <div class="place-content">
        <div class="place-title">9. Leh-Ladakh</div>
        <p class="place-desc">A paradise for adventure seekers, Leh-Ladakh offers breathtaking landscapes, high mountain passes, monasteries, and unique Tibetan culture.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
     <div class="place">
        <a href="Discover more.html">
      <img src="https://himachaltourisminfoblog.com/wp-content/uploads/2024/04/Sissu_leh_ladakh-1895x760.jpg" alt="Leh-Ladakh">
        </a>
      <div class="place-content">
        <div class="place-title">10. Leh-Ladakh</div>
        <p class="place-desc">A paradise for adventure seekers, Leh-Ladakh offers breathtaking landscapes, high mountain passes, monasteries, and unique Tibetan culture.</p>
      <a href="trip_detail.html" class="btn btn-primary">Book trip</a>
      </div>
    </div>
  </div>

  <footer>
    <div>Made with <i class="fa fa-heart" style="color:#e57373"></i> | Explore India | &copy; 2025</div>
    <div class="footer-social">
      <a href="https://www.instagram.com/" title="Instagram"><i class="fab fa-instagram"></i></a>
      <a href="https://www.facebook.com/" title="Facebook"><i class="fab fa-facebook"></i></a>
      <a href="https://x.com/?lang=en" title="Twitter"><i class="fab fa-twitter"></i></a>
    </div>
  </footer>

  <script>
    const menuBtn = document.querySelector('.menu-btn');
    const navLinks = document.querySelector('.nav-links');
    menuBtn.onclick = () => {
      navLinks.classList.toggle('show');
    };
  </script>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
