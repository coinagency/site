<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dewar Production | Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
<style>
/* ===== GLOBAL ===== */
body, html {
  margin: 0;
  padding: 0;
  width: 100%;
  font-family: 'Inter', sans-serif;
  background: #0a0a0f;
  color: #fff;
  line-height: 1.6;
}

/* VARIABLES DE COULEURS */
:root {
  --bg-soft: #12121a;
  --text: #ffffff;
  --muted: #b0b0c1;
  --accent: #4f7cff;
  --accent2: #9b6cff;
  --gold: #f5c542;
  --highlight: #ff6f61;
  --grad-btn: linear-gradient(90deg, #4f7cff, #9b6cff);
}

/* ===== ECRAN DECOUVRIR ===== */
#welcome {
  position: fixed;
  top: 0; left: 0;
  width:100%; height:100%;
  background: linear-gradient(135deg, #0a0a0f, #1b1b25);
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

#welcome h1 {
  font-size: 64px;
  margin-bottom: 18px;
  font-weight: 700;
  color: var(--accent);
}

#discoverBtn {
  padding: 18px 60px;
  font-size: 32px;
  font-weight: 700;
  border: none;
  border-radius: 50px;
  background: var(--grad-btn);
  color: #fff;
  cursor: pointer;
  transition: transform 0.3s, box-shadow 0.3s;
  box-shadow: 0 0 25px rgba(79,124,255,0.6);
}

#discoverBtn:hover {
  transform: scale(1.08);
  box-shadow: 0 0 45px rgba(155,108,255,0.8);
}

/* ===== SITE ===== */
#site { display: none; width: 100%; }

/* SECTIONS */
section {
  padding: 60px 30px;
  max-width: 1200px;
  margin: auto;
}

h1,h2,h3 {
  margin: 0 0 18px 0;
  font-weight: 700;
  opacity: 0;
  animation: fadeIn 1s forwards;
}

h1 { font-size: 56px; text-align: center; color: var(--accent); animation-delay: 0.4s; }
h2 { font-size: 42px; color: var(--highlight); animation-delay: 0.6s; }
h3 { font-size: 30px; color: var(--accent2); animation-delay: 0.8s; }

p { color: var(--muted); font-size: 18px; margin-bottom: 15px; }
ul { margin-left: 20px; color: var(--muted); }

/* ===== STATS GRID ===== */
.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(200px,1fr));
  gap: 25px;
  text-align: center;
  margin-top: 30px;
  margin-bottom: 30px;
}

.stat-card {
  background: var(--bg-soft);
  border-radius: 16px;
  padding: 30px 20px;
  transition: transform 0.3s, box-shadow 0.3s;
  opacity: 0;
  animation: fadeInUp 1s forwards;
}

.stat-card:hover {
  transform: translateY(-10px) scale(1.05);
  box-shadow: 0 0 25px rgba(79,124,255,0.6);
}

.stat-number {
  font-size: 40px;
  font-weight: 700;
  color: var(--accent);
  margin-bottom: 8px;
}

.stat-label {
  font-size: 18px;
  font-weight: 600;
  color: var(--text);
}

/* GRID CLIENTS */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
  gap: 30px;
  margin-top: 30px;
}

.card {
  background: var(--bg-soft);
  border-radius: 18px;
  overflow: hidden;
  text-align: center;
  padding: 15px;
  opacity: 0;
  animation: fadeInUp 1s forwards;
  transition: transform 0.3s, box-shadow 0.3s;
}

.card img { width: 100%; border-radius: 12px; }
.card .name { margin-top: 14px; font-size: 18px; font-weight: 600; color: var(--accent); }
.card .views { margin-top: 6px; font-size: 14px; color: var(--muted); }

.card:hover {
  transform: translateY(-8px) scale(1.04);
  box-shadow: 0 0 25px rgba(79,124,255,0.5);
}

/* REVIEWS */
.reviews {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
  gap: 28px;
  margin-top: 20px;
}

.review {
  background: var(--bg-soft);
  padding: 22px;
  border-radius: 14px;
  opacity: 0;
  animation: fadeIn 1s forwards;
}

.review .stars { color: var(--gold); font-size: 18px; margin-bottom: 8px; }
.review p { color: var(--muted); font-size: 16px; }

/* FOOTER */
footer { text-align:center; padding:25px; color: var(--muted); font-size: 13px; }

/* ANIMATIONS */
@keyframes fadeIn { from { opacity:0; transform: translateY(10px); } to { opacity:1; transform: translateY(0); } }
@keyframes fadeInUp { from { opacity:0; transform: translateY(30px); } to { opacity:1; transform: translateY(0); } }
</style>
</head>

<body>

<!-- ECRAN DECOUVRIR -->
<div id="welcome">
  <h1>Bienvenue chez Dewar Production</h1>
  <button id="discoverBtn">Découvrir</button>
</div>

<!-- CONTENU DU SITE -->
<div id="site">

  <!-- STATS KEY BLOCK -->
  <section>
    <h2 style="text-align:center; color:var(--accent2); margin-bottom:40px;">Dewar Production en chiffres</h2>
    <div class="stats-grid">
      <div class="stat-card">
        <div class="stat-number">+10</div>
        <div class="stat-label">Personnes accompagnées</div>
      </div>
      <div class="stat-card">
        <div class="stat-number">1M</div>
        <div class="stat-label">Vues générées</div>
      </div>
      <div class="stat-card">
        <div class="stat-number">5+</div>
        <div class="stat-label">Contacts clés</div>
        <p style="font-size:14px; color:var(--muted); margin-top:5px;">
          Keo, Marcus Lawrence, Blyatt, Stéphane Matalla et d'autres
        </p>
      </div>
      <div class="stat-card">
        <div class="stat-number">5 ans</div>
        <div class="stat-label">d’expertise</div>
      </div>
    </div>
  </section>

  <!-- VIDEOS CLIENTS -->
  <section>
    <h3>Mes meilleures collaborations</h3>
    <div class="grid">
      <a class="card" href="https://youtu.be/fc8H7MgbbFE" target="_blank">
        <img src="https://img.youtube.com/vi/fc8H7MgbbFE/maxresdefault.jpg" alt="Stéphane Matalla">
        <div class="name">Stéphane Matalla</div>
        <div class="views">55 000 vues</div>
      </a>

      <a class="card" href="https://youtu.be/dVAm_Ay3fXM?list=TLPQMjkxMjIwMjWNpDC5-JKl0g" target="_blank">
        <img src="https://img.youtube.com/vi/dVAm_Ay3fXM/maxresdefault.jpg" alt="Blyatt">
        <div class="name">Blyatt</div>
        <div class="views">22 000 vues</div>
      </a>

      <a class="card" href="https://youtu.be/SI34h2IRUgA" target="_blank">
        <img src="https://img.youtube.com/vi/SI34h2IRUgA/maxresdefault.jpg" alt="Dewar">
        <div class="name">Dewar</div>
        <div class="views">600 vues</div>
      </a>
    </div>
  </section>

  <!-- AVIS CLIENTS -->
  <section>
    <h3>Avis clients</h3>
    <div class="reviews">
      <div class="review">
        <div class="stars">★★★★★</div>
        <p>Montage ultra professionnel, rythmé et engageant — hautement recommandé.</p>
      </div>

      <div class="review">
        <div class="stars">★★★★★</div>
        <p>Très bonne communication et rendu au‑delà de nos attentes.</p>
      </div>

      <div class="review">
        <div class="stars">★★★★★</div>
        <p>Dewar sait comment raconter une histoire visuelle — un vrai pro.</p>
      </div>
    </div>
  </section>

  <!-- SECTION CONTACT -->
  <section style="text-align:center; margin-top:50px; margin-bottom:30px;">
    <h3 style="color:var(--accent2); margin-bottom:15px;">Contactez-moi</h3>
    <p style="color:var(--muted); font-size:18px; margin-bottom:8px;">
      Instagram : <a href="https://instagram.com/arno.dwe" target="_blank" style="color:var(--highlight); text-decoration:none;">@arno.dwe</a>
    </p>
    <p style="color:var(--muted); font-size:18px; margin-bottom:8px;">
      Téléphone : <a href="tel:+33786705803" style="color:var(--highlight); text-decoration:none;">07 86 70 58 03</a>
    </p>
    <p style="color:var(--muted); font-size:18px;">
      Mail : <a href="mailto:contact.dewarr@gmail.com" style="color:var(--highlight); text-decoration:none;">contact.dewarr@gmail.com</a>
    </p>
  </section>

  <!-- FOOTER -->
  <footer>
    © Dewar production — Tous droits réservés
  </footer>

</div>

<script>
// Découvrir
document.getElementById('discoverBtn').addEventListener('click', () => {
  document.getElementById('welcome').style.display = 'none';
  document.getElementById('site').style.display = 'block';
});
</script>

</body>
</html>
