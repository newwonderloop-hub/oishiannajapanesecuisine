# oishiannajapanesecuisine
[index.html](https://github.com/user-attachments/files/25320574/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Oishi Japanese Cuisine</title>
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>

/* ========== FONT ========== */
@font-face {
  font-family: 'Japanese3017';
  src: url("font/Japanese 3017.otf");
}

/* ========== RESET ========== */
*{
 margin:0;
 padding:0;
 box-sizing:border-box;
}

body{
 font-family:Arial, sans-serif;
 background: linear-gradient(-45deg, #0b0b1f, #120a3d, #0b0b1f, #07070f);
 background-size:400% 400%;
 animation: neon-bg 15s ease infinite;
 color:white;
 scroll-behavior:smooth;
}

/* ========== NEON BG ========== */
@keyframes neon-bg {
  0%{background-position:0% 50%;}
  50%{background-position:100% 50%;}
  100%{background-position:0% 50%;}
}

/* ========== NAV ========== */
nav{
 position:fixed;
 width:100%;
 top:0;
 background:#111;
 padding:15px;
 text-align:center;
 z-index:999;
}
nav a{
 color:white;
 margin:0 15px;
 text-decoration:none;
 font-weight:bold;
 text-shadow:0 0 6px #0ff;
 transition:0.3s;
}
nav a:hover{
 color:#0ff;
 text-shadow:
   0 0 8px #0ff,
   0 0 15px #00bfff;
}

/* ========== HEADER ========== */
#home{
 width:100%;
 height:480px;
 background:url("images/header1.jpg") center/cover no-repeat;
 display:flex;
 justify-content:center;
 align-items:center;
 text-align:center;
}
#home .box{
 background:rgba(0,0,0,0.6);
 padding:20px 40px;
 border-radius:12px;
}
#home h1{
 font-family:'Japanese3017';
 font-size:48px;
 color:#0ff;
 text-shadow: 
   0 0 10px #0ff, 
   0 0 20px #0ff, 
   0 0 30px #00bfff;
 animation: flicker 1.5s infinite alternate;
}
@keyframes flicker {
  from { text-shadow:0 0 10px #0ff,0 0 20px #0ff; }
  to   { text-shadow:0 0 15px #0ff,0 0 30px #00bfff; }
}
#home p{margin-top:10px;font-size:20px;color:#fff;}

/* ========== MENU ========== */
section{
 padding:90px 20px;
 text-align:center;
}
.menu-grid{
 display:grid;
 grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
 gap:18px;
 max-width:900px;
 margin:auto;
}
.menu-grid img{
 width:100%;
 border-radius:10px;
 box-shadow:
   0 0 8px #0ff,
   0 0 15px #00bfff;
 transition:0.3s;
}
.menu-grid img:hover{
 transform:scale(1.06);
 box-shadow: 
   0 0 12px #0ff,
   0 0 20px #00bfff;
}

/* ========== CUSTOMER GALLERY ========== */
.gallery-grid{
 display:grid;
 grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
 gap:15px;
 max-width:1000px;
 margin:auto;
}
.gallery-grid img{
 width:100%;
 border-radius:10px;
 box-shadow:
   0 0 8px #0ff,
   0 0 15px #00bfff;
 transition:0.3s ease;
 cursor:pointer;
}
.gallery-grid img:hover{
 transform:scale(1.08);
 box-shadow:
   0 0 12px #0ff,
   0 0 20px #00bfff;
}

/* ========== SOCIAL & CONTACT ========== */
.social-icons{
 display:flex;
 justify-content:center;
 gap:25px;
 flex-wrap:wrap;
 margin-top:20px;
}
.social-icons a{
 text-decoration:none;
 color:white;
 font-size:18px;
 display:flex;
 align-items:center;
 gap:8px;
 padding:8px 14px;
 border-radius:8px;
 transition:0.3s;
}
.social-icons a:hover{
 background:rgba(0,255,255,0.2);
 transform:scale(1.1);
}
.social-icons img{
 width:42px;
}

/* ========== MAP ========== */
iframe{
 width:90%;
 max-width:800px;
 height:320px;
 border:none;
 border-radius:12px;
 margin-top:15px;
}

/* ========== REVIEWS ========== */
.review{
 background:#171717;
 padding:18px;
 border-radius:10px;
 margin:15px auto;
 max-width:600px;
}
.stars{
 color:gold;
 font-size:22px;
 margin-bottom:8px;
}

/* ========== FOOTER ========== */
footer{
 background:#111;
 padding:20px;
 text-align:center;
}

</style>
</head>

<body>

<nav>
 <a href="#home">Home</a>
 <a href="#menu">Menu</a>
 <a href="#gallery">Gallery</a>
 <a href="#social">Social</a>
 <a href="#location">Location</a>
 <a href="#reviews">Reviews</a>
</nav>

<section id="home">
 <div class="box">
   <h1>OISHI JAPANESE CUISINE</h1>
   <p>Bringing The Art Of Japanese Hibachi And Sushi To The. Street-Crafted with Precision Served With Passion</p>
 </div>
</section>

<section id="menu">
 <h2>Our Menu</h2>
 <div class="menu-grid">
   <img src="images/menu1.jpg">
   <img src="images/menu2.jpg">
 </div>
</section>


<section id="gallery">
 <h2>Customer Gallery 📸</h2>
 <div class="gallery-grid">
   <img src="images/customer1.jpg" alt="Customer 1">
   <img src="images/customer2.png" alt="Customer 2">
   <img src="images/customer3.jpeg" alt="Customer 3">
   <img src="images/customer4.jpg" alt="Customer 4">
 </div>
</section>

<section id="social">
 <h2>Follow & Contact Us</h2>
 <div class="social-icons">
   <a href="https://facebook.com/yourpage" target="_blank">
     <img src="images/logo-facebook.png">Oishi Anna
   </a>
   <a href="https://instagram.com/yourpage" target="_blank">
     <img src="images/logo-instagram.png">oishi.anna
   </a>
   <a href="https://tiktok.com/@yourpage" target="_blank">
     <img src="images/logo-tiktok.png">oishianna
   </a>
   <a href="https://youtube.com/yourchannel" target="_blank">
     <img src="images/logo-youtube.png">@oisihiJapaneseCuisine
   </a>
 </div>

 <div class="social-icons" style="margin-top:12px;">
   <a href="tel:+15735760771">
     <img src="images/logo-telephone.png">+1 573 576 0441
   </a>
   <a href="mailto:youremail@example.com">
     <img src="images/logo-email.png">oishiannajapanesecuisine.com
   </a>
 </div>
</section>

<section id="location">
 <h2>Our Location 📍</h2>
 <p>219 E Vieeanna, Anna, Illinois 62906 USA</p>
 <iframe src="https://maps.google.com/maps?q=219%20E%20Vieeanna%20Anna%20Illinois%2062906%20USA&output=embed"></iframe>
</section>

<section id="reviews">
  <h2>Customer Reviews ⭐⭐⭐⭐⭐</h2>

  <div class="review">
    <div class="stars">★★★★★</div>
    <p>Amazing sushi & service! Best experience ever!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★☆</div>
    <p>Great hibachi and atmosphere!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★★</div>
    <p>I keep coming back for the sushi rolls — delicious!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★★</div>
    <p>Friendly staff and authentic flavors! Highly recommended!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★☆</div>
    <p>Loved the hibachi — amazing presentation and taste.</p>
  </div>

  <div class="review">
    <div class="stars">★★★★★</div>
    <p>Amazing sashimi! Fresh and tasty every time!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★☆</div>
    <p>Good portions and great price — will visit again!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★★</div>
    <p>One of the best Japanese food trailers in town!</p>
  </div>

  <div class="review">
    <div class="stars">★★★★★</div>
    <p>Love the atmosphere — cozy and fun dining experience.</p>
  </div>

  <div class="review">
    <div class="stars">★★★★☆</div>
    <p>A solid 4 stars! Good food, nice staff.</p>
  </div>

</section>

<footer>
 © 2026 Oishi Japanese Cuisine Hibachi And Sushi
</footer>

</body>
</html>
