<template>
  <div class="">
    <div class="hero-section">
      <div class="container">
        <h1>Mondano</h1>
        <p class="subtitle">Convirtiendo sueños de moda en realidad</p>
        <!-- <div class="social-links">
          <font-awesome-icon :icon="['fab', 'fa-linkedin']" /><a href="www.linkedin.com">linkedin</a>
        </div> -->
      </div>
    </div>
    <!-- Hero Section -->

    <!-- About Section -->
    <div class="container py-5">
      <div class="">
        <span class="badge">QUIÉNES SOMOS</span>
        <!-- <h2>Sobre Nosotros</h2> -->
      </div>
      <div class="about-content">
        <div class="row">
          <div class="col-md-6">
            <!-- <img src="@/assets/images/about-image.jpg" alt="Sobre Mondano" class="about-image" /> -->
          </div>
          <div class="col-md-6">
            <p class="about-text">
              Mondano es una empresa líder en moda dedicada a crear ropa y accesorios modernos y con estilo. Con años de
              experiencia en la industria de la moda, hemos construido nuestra reputación basada en la calidad y la
              innovación.
            </p>
            <div class="info-grid">
              <div class="info-item"><span>Ubicación:</span> Chile</div>
              <div class="info-item"><span>Fundada:</span> 2015</div>
            </div>
          </div>
        </div>
      </div>

      <!-- Video Section -->
      <div class="video-section">
        <div class="video-container mb-5">
          <video controls class="responsive-video mb-4">
            <source src="@/assets/videos/video_1.mp4" type="video/mp4" />
            Tu navegador no soporta el elemento de video.
          </video>

          <video controls class="responsive-video">
            <source src="@/assets/videos/video_2.mp4" type="video/mp4" />
            Tu navegador no soporta el elemento de video.
          </video>
        </div>
      </div>
    </div>

    <!-- Footer Section -->
    <footer class="footer-section">
      <div class="container">
        <div class="footer-content">
          <div class="footer-grid">
            <div class="footer-column">
              <h3>Mondano</h3>
              <p>Innovación y estilo en cada detalle. Creando tendencias desde 2015.</p>
            </div>

            <!-- <div class="footer-column">
              <h4>Contacto</h4>
              <ul>
                <li><font-awesome-icon :icon="['fas', 'location-dot']" /> Santiago, Chile</li>
                <li><font-awesome-icon :icon="['fas', 'phone']" /> +56 2 2345 6789</li>
                <li><font-awesome-icon :icon="['fas', 'envelope']" /> contacto@mondano.cl</li>
              </ul>
            </div> -->

            <!-- <div class="footer-column">
              <h4>Síguenos</h4>
              <div class="social-icons">
                <a href="#"><font-awesome-icon :icon="['fab', 'instagram']" /></a>
                <a href="#"><font-awesome-icon :icon="['fab', 'facebook']" /></a>
                <a href="#"><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
              </div>
            </div> -->
          </div>

          <div class="footer-bottom">
            <p>&copy; 2025 Claudio Rojas Alarcon. Todos los derechos reservados.</p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
// Component logic here
</script>

<style scoped>
.hero-section {
  background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url("@/assets/images/hero-bg.jpg");
  background-size: cover;
  background-position: center;
  height: 100vh;
  display: flex;
  align-items: center;
  text-align: center;
  color: white;
}

.hero-section h1 {
  font-size: 3.5rem;
  font-weight: bold;
  margin-bottom: 1rem;
}

.subtitle {
  font-size: 1.2rem;
  margin-bottom: 2rem;
}

.social-links a {
  color: white;
  margin: 0 10px;
  font-size: 1.5rem;
}

.section {
  padding: 100px 0;
}

.section-header {
  text-align: center;
  margin-bottom: 50px;
}

.badge {
  background: #007bff;
  color: white;
  padding: 5px 15px;
  border-radius: 20px;
  margin-bottom: 15px;
  display: inline-block;
}

.about-image {
  width: 100%;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.about-text {
  margin: 20px 0;
  line-height: 1.8;
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 30px;
}

.info-item span {
  font-weight: bold;
  color: #007bff;
}

.video-container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}

.responsive-video {
  width: 100%;
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  margin-bottom: 30px;
}

.footer-section {
  background-color: #1a1a1a;
  color: #ffffff;
  padding: 60px 0 20px;
  margin-top: 60px;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
}

.footer-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 40px;
  margin-bottom: 40px;
}

.footer-column h3 {
  font-size: 1.8rem;
  margin-bottom: 20px;
  color: #ffffff;
}

.footer-column h4 {
  font-size: 1.2rem;
  margin-bottom: 20px;
  color: #007bff;
}

.footer-column p {
  line-height: 1.6;
  color: #cccccc;
}

.footer-column ul {
  list-style: none;
  padding: 0;
}

.footer-column ul li {
  margin-bottom: 15px;
  color: #cccccc;
  display: flex;
  align-items: center;
  gap: 10px;
}

.social-icons {
  display: flex;
  gap: 20px;
}

.social-icons a {
  color: #ffffff;
  font-size: 1.5rem;
  transition: color 0.3s ease;
}

.social-icons a:hover {
  color: #007bff;
}

.footer-bottom {
  text-align: center;
  padding-top: 20px;
  border-top: 1px solid #333;
  color: #888;
}

@media (max-width: 768px) {
  .footer-grid {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .footer-column ul li {
    justify-content: center;
  }

  .social-icons {
    justify-content: center;
  }
}
</style>
