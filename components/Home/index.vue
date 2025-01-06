<template>
  <div class="container">
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light py-3">
      <div class="container-fluid">
        <a class="navbar-brand fw-bold" href="#"> <span class="text-primary">CR</span> Claudio Rojas Alarcon </a>
        <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
          <span class="navbar-toggler-icon"></span>
        </button> -->
        <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
          <ul class="navbar-nav">
            <ul class="navbar-nav">
              <li class="nav-item"><NuxtLink class="nav-link" to="/">Inicio</NuxtLink></li>
              <li class="nav-item"><NuxtLink class="nav-link" to="/empresas">Empresas</NuxtLink></li>
              <li class="nav-item"><NuxtLink class="nav-link" to="/proyectos">Proyectos futuros</NuxtLink></li>
              <li class="nav-item"><NuxtLink class="nav-link" to="/contacto">Contacto</NuxtLink></li>
            </ul>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Hero Section -->
    <div class="row py-5 align-items-center">
      <div class="col-md-6">
        <h1 class="text-danger mb-2">Claudio Rojas Alarcón</h1>
        <h2 class="fw-bold mb-4">
          Una persona apasionada por la moda, actual CEO y CO-Founder de mondano.cl, donde canalizo mi creatividad y
          visión de diseño. Además, asesor de empresas en términos legales y financieros, aportando experiencia y
          estrategia en sus operaciones
        </h2>
        <button class="btn btn-danger px-4">Hablemos</button>
      </div>
      <div class="col-md-6 position-relative">
        <div class="gradient-overlay"></div>
        <img src="./../../assets/claudio-pic.jpeg" alt="Profile" class="img-fluid rounded position-relative" />
      </div>
    </div>

    <!-- Companies Section -->
    <div class="py-5">
      <h2 class="fw-bold mb-4 text-center"><span class="text-danger">Empresas</span> lideradas</h2>
      <div class="row g-4">
        <div class="col-md-4 offset-md-2">
          <div class="card shadow rounded">
            <div class="card-body">
              <h3 class="fw-bold mb-3">MONDANO</h3>
              <img src="./../../assets/mondano-logo.jpeg" alt="Mondano" class="img-fluid mb-3" />
              <p class="text-muted">Tienda online de ropa exclusiva - fabricación nacional</p>

              <a href="https://mondano.cl" target="_blank" class="btn btn-outline-danger">Visitar sitio</a>
            </div>
          </div>
        </div>
        <div class="col-md-4 offset-md-1">
          <div class="card shadow rounded">
            <div class="card-body">
              <h3 class="fw-bold mb-3">ELABORE</h3>
              <img src="./../../assets/elabore-chile.jpg" alt="Elabore" class="img-fluid mb-3" />
              <p class="text-muted">Fábrica téxtil en Chile dedicada a elaborar prendas de vestir de alta calidad.</p>
              <!-- <button class="btn btn-outline-danger">Visitar sitio</button> -->
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Values Section -->
    <div class="row">
      <div class="col-md-6 m-auto d-block text-center">
        <div class="py-5">
          <h2 class="fw-bold text-center mb-5">
            Mis <span class="text-primary">valores</span>, mi <span class="text-danger">horizonte</span>
          </h2>
          <div class="values-list">
            <div
              v-for="(n, index) in values"
              :key="n"
              :class="[
                'd-flex gap-4 mb-4',
                index % 2 === 0 ? 'flex-row align-items-center text-align-end' : 'flex-row-reverse',
              ]">
              <div
                :class="[
                  'rounded-circle align-items-center d-flex justify-content-center text-white',
                  index === 1 ? 'bg-danger' : index === 2 ? 'bg-purple' : index === 3 ? 'bg-primary' : 'bg-info',
                ]">
                {{ index + 1 }}
              </div>
              <p :class="['flex-grow-1 text-muted', index % 2 === 0 ? 'text-end' : 'text-start']">
                {{ values[index] }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Future Projects Section -->
    <div class="py-5">
      <div class="card bg-gradient shadow rounded">
        <div class="card-body">
          <div class="row align-items-center">
            <div class="col-md-6">
              <h2 class="fw-bold mb-3">Diseño e innovación</h2>
              <p class="text-muted font-size-lg">
                Mi misión es liderar mondano.cl con creatividad e innovación, ofreciendo diseños únicos que inspiran y
                empoderan a las personas. Paralelamente, brindo asesoría legal y financiera estratégica para impulsar el
                éxito y crecimiento sostenible de las empresas y que todos tengan la oportunidad de emprender en sus
                negocios.
              </p>
            </div>
            <div class="col-md-6">
              <img src="./../../assets/mision-claudio.jpeg" alt="Future projects" class="img-fluid rounded" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <section class="py-5">
      <h2 class="fw-bold mb-4">Trayectoria Profesional</h2>
      <p class="text-muted">
        Con más de una década de experiencia en la industria textil y moda, he liderado proyectos innovadores que han
        transformado el panorama de la moda en Chile. Como CEO de Mondano, hemos logrado crear una marca que no solo
        representa estilo, sino también valores de sostenibilidad y producción local.
      </p>
      <p class="text-muted">
        Mi experiencia en asesoría empresarial abarca desde startups hasta empresas establecidas, ayudándolas a
        optimizar sus operaciones y alcanzar sus objetivos estratégicos. He trabajado con más de 50 empresas,
        implementando soluciones efectivas en áreas legales y financieras.
      </p>
    </section>

    <!-- Expertise Section -->
    <section class="py-5">
      <h2 class="fw-bold mb-4">Áreas de Especialización</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card h-100">
            <div class="card-body">
              <h3 class="h5 mb-3">Gestión Empresarial</h3>
              <p>
                Desarrollo de estrategias de negocio, optimización de procesos y gestión de equipos multidisciplinarios.
                Experiencia en planificación estratégica y toma de decisiones ejecutivas.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card h-100">
            <div class="card-body">
              <h3 class="h5 mb-3">Industria Textil</h3>
              <p>
                Conocimiento profundo de la cadena de suministro textil, procesos de producción y control de calidad.
                Desarrollo de colecciones y gestión de marca en el mercado de la moda.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card h-100">
            <div class="card-body">
              <h3 class="h5 mb-3">Asesoría Legal y Financiera</h3>
              <p>
                Consultoría especializada en aspectos legales y financieros para empresas en crecimiento. Experiencia en
                estructuración de negocios y optimización fiscal.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <footer>
      <p>&copy; 2025 Claudio Rojas Alarcón</p>
      <ul>
        <li><a href="https://es-la.facebook.com/klauRoj" target="_blank">Facebook</a></li>
        <li><a href="https://www.instagram.com/klaudioroj/" target="_blank">Instagram</a></li>
        <li><a href="https://www.linkedin.com/in/fabrica-texti-84ba33155/" target="_blank">Linkdin</a></li>
      </ul>
    </footer>
  </div>
</template>

<script lang="ts">
export default {
  name: "HomeComponent",
  template: "HomeComponent",
};
</script>

<script setup lang="ts">
const values = ref([
  "Integridad y transparencia en cada proyecto que emprendo",
  "Innovación constante en el desarrollo de soluciones",
  "Compromiso con la calidad y satisfacción del cliente",
  "Responsabilidad social y desarrollo sostenible",
]);
</script>

<style scoped>
.gradient-overlay {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background: linear-gradient(45deg, rgba(0, 123, 255, 0.5), rgba(220, 53, 69, 0.5));
  border-radius: 0.25rem;
  z-index: 1;
}

.img-fluid {
  z-index: 2;
}
.bg-purple {
  background-color: #9333ea;
}

.bg-gradient {
  background: linear-gradient(to right, #e9d5ff, #fbcfe8);
}

/* Custom utilities */
.gap-4 {
  gap: 1.5rem;
}

.rounded-circle {
  border-radius: 50%;
  width: 10vh;
  height: 5vh;
  font-size: 1.5rem;
}

.card img {
  width: 30vh;
}

/* Ensure proper spacing on mobile */
@media (max-width: 768px) {
  .values-list > div {
    margin-bottom: 2rem;
  }
}
</style>
