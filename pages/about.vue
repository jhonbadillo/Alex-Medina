<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Somos Santander"
      subtitle="Desarrollo de actividades del Diputado Alexander Medina"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>¿Quien soy?</h3>
          <p>
            <strong>
              Conoce quien es Noe Alexander Medina.
            </strong>
          </p>
          <p>
            Nací en Bolívar Santander, el 3 de febrero 1973. Hijo de Noé Medina 
            y Bárbara Sosa, padres Educadores, soy el mayor de 4 hermanos, Mi hermosa 
            familia está conformada por mi esposa Dora Emilce Moreno Vargas y mis Hijos 
            María Alejandra, Karen Daniela y David Steban. Realice mis estudios de primaria 
            y bachillerato en el Colegio Integrado Simón Bolívar en el municipio de Bolívar Santander.
          </p>

          <h3>Estudios</h3>
          <p>
            Soy Administrador de Empresas y Empresario en el Gremio de Distribución de productos 
            de aseo y alimentos para el canal de tiendas.
          </p>
          <quote-card />
          <h3>Experiencia</h3>
          <p>
            Trabajé como Técnico Administrativo en el Hospital del municipio de Bolívar 
            en el periodo comprendido del 1 de julio 1993 a 20 de diciembre 2004, fui 
            Alcalde del municipio de Bolívar Santander en el periodo 2008 – 2011.
          </p>
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Ultimas publicaciones
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
