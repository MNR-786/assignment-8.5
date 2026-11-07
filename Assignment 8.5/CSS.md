* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  color: #24352f;
  background: #f5f6f2;
}

.site-layout {
  min-height: 100vh;
  display: grid;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    "header"
    "main"
    "footer";
}

.site-header {
  grid-area: header;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  padding: 18px max(24px, calc((100% - 1160px) / 2));
  border-bottom: 1px solid #e0e5dd;
  background: #fff;
}

.logo {
  color: #285b45;
  font-size: 1.5rem;
  font-weight: 800;
  text-decoration: none;
}

.logo span {
  color: #d47d4f;
}

.site-header nav {
  display: flex;
  flex-wrap: wrap;
  gap: 22px;
}

.site-header nav a {
  color: #52655b;
  text-decoration: none;
}

.main-content {
  grid-area: main;
  width: min(1160px, 100%);
  margin: 0 auto;
  padding: 42px 24px 56px;
}

.intro {
  margin-bottom: 28px;
  text-align: center;
}

.eyebrow {
  margin: 0 0 8px;
  color: #bd6b40;
  font-size: 0.76rem;
  font-weight: bold;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}

.intro h1 {
  margin: 0;
  font-size: clamp(2rem, 5vw, 3.2rem);
}

.intro > p:last-child {
  margin: 10px 0 0;
  color: #68796f;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  grid-template-areas:
    "feature feature image-two image-three"
    "image-four image-five last last";
  gap: 18px;
}

.gallery-card {
  position: relative;
  min-width: 0;
  height: 250px;
  margin: 0;
  overflow: hidden;
  border-radius: 13px;
  background: #dce4df;
}

.gallery-card img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}

.gallery-card:hover img {
  transform: scale(1.04);
}

.gallery-card figcaption {
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
  padding: 42px 16px 15px;
  overflow-wrap: anywhere;
  color: #fff;
  background: linear-gradient(transparent, #10241ddd);
}

.gallery-card figcaption span {
  font-size: 0.72rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.gallery-card h2 {
  margin: 4px 0 0;
  font-size: 1.2rem;
}

.feature-card {
  grid-area: feature;
  height: 320px;
}

.gallery-card:nth-child(2) {
  grid-area: image-two;
}

.gallery-card:nth-child(3) {
  grid-area: image-three;
}

.gallery-card:nth-child(4) {
  grid-area: image-four;
}

.gallery-card:nth-child(5) {
  grid-area: image-five;
}

.feature-card-last {
  grid-area: last;
}

.site-footer {
  grid-area: footer;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 10px 20px;
  padding: 18px max(24px, calc((100% - 1160px) / 2));
  background: #28513f;
  color: #fff;
  font-size: 0.9rem;
}

.site-footer p {
  margin: 0;
}

@media (max-width: 850px) {
  .gallery-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
    grid-template-areas:
      "feature feature"
      "image-two image-three"
      "image-four image-five"
      "last last";
  }

  .gallery-card,
  .feature-card {
    height: 260px;
  }
}

@media (max-width: 520px) {
  .site-header {
    flex-wrap: wrap;
    justify-content: center;
    padding: 16px;
  }

  .main-content {
    padding: 32px 14px 40px;
  }

  .gallery-grid {
    grid-template-columns: minmax(0, 1fr);
    grid-template-areas:
      "feature"
      "image-two"
      "image-three"
      "image-four"
      "image-five"
      "last";
    gap: 14px;
  }

  .gallery-card,
  .feature-card {
    height: 230px;
  }

  .site-footer {
    flex-direction: column;
    align-items: center;
    padding: 18px;
    text-align: center;
  }
}