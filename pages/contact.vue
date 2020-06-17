<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
    <site-hero
      title="Contactenos"
      subtitle="Listos para escucharte"
      image="/uploads/contact-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Hola!
              </p>
              <p class="subtitle">
                Que puedo hacer por ti?
              </p>
              <figure class="image is-1by1 ">
                <opti-image
                  :src="require('~/assets/uploads/noe.jpg').src"
                  :srcset="
                    require('~/assets/uploads/noe.jpg').srcSet
                  "
                />
              </figure>
              <br />
              <div class="content">
                <p>
                  <strong>
                    mi objetivo es ser <code>gestor </code>de proyectos incluyentes para toda la comunidad.
                  </strong>
                </p>
                <p>
                  Nací en Bolívar Santander, el 3 de febrero 1973. 
                  Hijo de Noé Medina y Bárbara Sosa, padres Educadores, 
                  soy el mayor de 4 hermanos, Mi hermosa familia está 
                  conformada por mi esposa Dora Emilce Moreno Vargas 
                  y mis Hijos María Alejandra, Karen Daniela y David Steban. 
                  Realice mis estudios de primaria y bachillerato en el 
                  Colegio Integrado Simón Bolívar en el municipio de Bolívar Santander.
                </p>
              </div>
            </article>
          </div>
          <div class="tile is-parent is-8">
            <article class="tile is-child box">
              <contact-form />
            </article>
          </div>
        </div>
      </template>
      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Ultimas Publicaciones
        </h3>
        <!-- Latest Posts -->
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import ContactForm from '~/components/ContactForm'
export default {
  head() {
    return {
      title: `Contact | ${this.$siteConfig.siteName}`
    }
  },
  components: { ContactForm }
}
</script>
