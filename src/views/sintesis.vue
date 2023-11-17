<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .row.justify-content-center.mt-5
      .col-lg-10.mb-5(data-aos="fade-right")
        figure
          img(src="@/assets/curso/sintesis.svg", alt="La síntesis resume todos los temas y subtemas abordados en el desarrollo del componente formativo; para este caso se aboró los tipos de experiencias gastronómicas que existen, coo se debe determinar este tipo de experiencias, las claves y pasos a tener en cuenta para una experiencia memorable en el área de la gastronomía que sea inolvidable para el turista.")
      .col-auto(data-aos="fade-left")
        a.anexo.mb-4(:href="obtenerLink('/downloads/sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
