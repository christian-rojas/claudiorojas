<template>
  <main class="">
    <section class="container my-5">
      <h2 class="text-center mb-4">Sobre mí</h2>
      <div class="row">
        <div class="col-md-4">
          <div class="card h-100">
            <img
              src="./../../assets/claudio-pic.jpeg"
              width="100"
              height="100"
              class="card-img-top"
              alt="claudio-rojas-alarcon" />
            <div class="card-body">
              <h5 class="card-title">Quien soy?</h5>
              <p class="card-text">
                una persona apasionada por la moda, actual CEO y CO-Founder de mondano.cl, donde canalizo mi creatividad
                y visión de diseño. Además, asesor de empresas en términos legales y financieros, aportando experiencia
                y estrategia en sus operaciones.
              </p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card h-100">
            <div class="card-body">
              <h5 class="card-title">Mi misión</h5>
              <p class="card-text">
                Mi misión es liderar mondano.cl con creatividad e innovación, ofreciendo diseños únicos que inspiran y
                empoderan a las personas. Paralelamente, brindo asesoría legal y financiera estratégica para impulsar el
                éxito y crecimiento sostenible de las empresas y que todos tengan la oportunidad de emprender en sus
                negocios.
              </p>
              <img
                src="./../../assets/mision-claudio.png"
                width="100"
                height="100"
                class="card-img-top"
                alt="claudio-rojas-alarcon" />
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card h-100">
            <div class="card-body">
              <h5 class="card-title">¿Que hago?</h5>
              <p class="card-text">
                Lidero mondano.cl como CEO, desarrollando y gestionando una marca de moda que refleja creatividad y
                estilo. Además, asesoro empresas en temas legales y financieros, ayudándolas a optimizar sus operaciones
                y alcanzar sus objetivos estratégicos.
              </p>
              <img
                src="./../../assets/que-hago.png"
                width="100"
                height="100"
                class="card-img-top"
                alt="claudio-rojas-alarcon" />
            </div>
          </div>
        </div>
      </div>
      <div class="row mt-5 mb-5">
        <div class="container">
          <h2 class="text-center mb-4">Mis proyectos</h2>
          <div class="row">
            <div class="col-md-6">
              <div class="card mb-3">
                <div class="card-body">
                  <img
                    src="./../../assets/elabore-chile.jpg"
                    width="100"
                    height="100"
                    class="card-img-top"
                    alt="claudio-rojas-alarcon" />
                  <h5 class="card-title">Elabore</h5>
                  <p class="card-text">Fábrica téxtil en Chile dedicada a elaborar prendas de vestir de alta calidad</p>
                </div>
              </div>
            </div>
            <div class="col-md-6">
              <div class="card mb-3">
                <div class="card-body">
                  <img
                    src="./../../assets/mondano-logo.png"
                    width="100"
                    height="100"
                    class="card-img-top"
                    alt="claudio-rojas-alarcon" />
                  <h5 class="card-title">Mondano</h5>
                  <p class="card-text">Tienda online de venta de ropa exclusiva de fabricación nacional</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- <FeedbackComponent /> -->

    <footer>
      <p>&copy; 2025 Claudio Rojas Alarcon</p>
      <ul>
        <li><a href="https://es-la.facebook.com/klauRoj" target="_blank">Facebook</a></li>
        <li><a href="https://www.instagram.com/klaudioroj/" target="_blank">Instagram</a></li>
        <li><a href="https://www.linkedin.com/in/fabrica-texti-84ba33155/" target="_blank">Linkdin</a></li>
      </ul>
    </footer>
  </main>
</template>

<script lang="ts">
import FeedbackComponent from "@/components/Feedback/index.vue";

export default {
  name: "HomeComponent",
  template: "HomeComponent",
  components: {
    FeedbackComponent,
  },
  data() {
    return {
      projects: [
        {
          title: "Project 1",
          description: "A wonderful project showcasing my skills.",
          image: "https://via.placeholder.com/150",
          link: "#",
        },
        {
          title: "Project 2",
          description: "Another project that I am proud of.",
          image: "https://via.placeholder.com/150",
          link: "#",
        },
        {
          title: "Project 3",
          description: "An example of creative work.",
          image: "https://via.placeholder.com/150",
          link: "#",
        },
      ],
    };
  },
  methods: {
    // Add your methods here},
  },
};
</script>

<style scoped>
.card img {
  height: 300px;
  object-fit: cover;
}
/* styles.css */

/* General */
</style>
