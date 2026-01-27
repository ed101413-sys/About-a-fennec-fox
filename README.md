<header class="hero-section">
  <div class="hero-overlay">
    <h1 class="vertical-text">日本 <br><span>2026</span></h1>
    <p>Japan: A Fusion of Tradition & Taste</p>
  </div>
</header>

<main class="bento-grid">
  <!-- Culture: Tradition -->
  <section class="item item-culture">
    <div class="content-box">
      <span class="tag">Culture</span>
      <h2>Shinto Roots</h2>
      <p>Ancient spirits in modern forests.</p>
    </div>
  </section>

  <!-- Food: Sushi -->
  <section class="item item-sushi">
    <div class="content-box">
      <span class="tag">Food</span>
      <h2>Edomae Sushi</h2>
      <p>Art on a plate.</p>
    </div>
  </section>

  <!-- Food: Ramen -->
  <section class="item item-ramen">
    <div class="content-box">
      <span class="tag">Food</span>
      <h2>Craft Ramen</h2>
      <p>Hearty noodles and broth.</p>
    </div>
  </section>

  <!-- Culture: Nature -->
  <section class="item item-nature">
    <div class="content-box">
      <span class="tag">Nature</span>
      <h2>Sakura</h2>
      <p>Spring's pink arrival.</p>
    </div>
  </section>
</main>
:root {
  --japan-red: #bc002d;
  --bg-light: #fdfaf5;
}

body {
  font-family: sans-serif;
  background-color: var(--bg-light);
  margin: 0;
}

/* Header with background image */
.hero-section {
  height: 400px;
  background: url('https://images.unsplash.com') center/cover;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
}

.hero-overlay {
  background: rgba(0, 0, 0, 0.4);
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.vertical-text {
  writing-mode: vertical-rl;
  font-size: 4rem;
  margin: 0 auto;
}

/* Bento Grid */
.bento-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 40px;
  max-width: 1200px;
  margin: -50px auto 0;
}

.item {
  height: 300px;
  border-radius: 15px;
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  color: white;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}

/* Updated Image URLs for JSFiddle */
.item-culture { background-image: linear-gradient(transparent, rgba(0,0,0,0.8)), url('https://images.unsplash.com'); }
.item-sushi { background-image: linear-gradient(transparent, rgba(0,0,0,0.8)), url('https://images.unsplash.com'); }
.item-ramen { background-image: linear-gradient(transparent, rgba(0,0,0,0.8)), url('https://images.unsplash.com'); }
.item-nature { background-image: linear-gradient(transparent, rgba(0,0,0,0.8)), url('https://images.unsplash.com'); }

.content-box { padding: 20px; }
.tag { background: var(--japan-red); padding: 3px 10px; border-radius: 5px; font-size: 12px; }
h2 { margin: 10px 0 5px; }
p { margin: 0; font-size: 14px; opacity: 0.9; }
