<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Wander — Photo Gallery</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="site-layout">
    <header class="site-header">
      <a class="logo" href="#">wander<span>.</span></a>
      <nav aria-label="Main navigation">
        <a href="#gallery">Gallery</a>
        <a href="#about">About</a>
      </nav>
    </header>

    <main class="main-content" id="gallery">
      <section class="intro" id="about">
        <p class="eyebrow">Places worth remembering</p>
        <h1>Views from the journey</h1>
        <p>A small collection of landscapes, quiet moments, and open spaces.</p>
      </section>

      <section class="gallery-grid" aria-label="Travel photo gallery">
        <figure class="gallery-card feature-card">
          <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=1200&q=80" alt="Mountain lake reflecting the surrounding peaks">
          <figcaption>
            <span>01 / Lakes</span>
            <h2>Still waters</h2>
          </figcaption>
        </figure>

        <figure class="gallery-card">
          <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=900&q=80" alt="Mountain peaks beneath a bright sky">
          <figcaption>
            <span>02 / Mountains</span>
            <h2>Above the clouds</h2>
          </figcaption>
        </figure>

        <figure class="gallery-card">
          <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=900&q=80" alt="Sunlight passing through a green forest">
          <figcaption>
            <span>03 / Forests</span>
            <h2>Into the green</h2>
          </figcaption>
        </figure>

        <figure class="gallery-card">
          <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=900&q=80" alt="Wide open landscape with mountains in the distance">
          <figcaption>
            <span>04 / Open land</span>
            <h2>Wide horizons</h2>
          </figcaption>
        </figure>

        <figure class="gallery-card">
          <img src="https://images.unsplash.com/photo-1470252649378-9c29740c9fa8?auto=format&fit=crop&w=900&q=80" alt="Golden light over a misty field at sunrise">
          <figcaption>
            <span>05 / Sunrises</span>
            <h2>First light</h2>
          </figcaption>
        </figure>

        <figure class="gallery-card feature-card feature-card-last">
          <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=1200&q=80" alt="A mountain lake beneath a warm evening sky">
          <figcaption>
            <span>06 / Evenings</span>
            <h2>Last light</h2>
          </figcaption>
        </figure>
      </section>
    </main>

    <footer class="site-footer">
      <p>© 2025 Wander Gallery</p>
      <p>Made for curious travelers.</p>
    </footer>
  </div>
</body>
</html>