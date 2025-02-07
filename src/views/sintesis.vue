<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-5 A continuación, se presenta una visión general sobre ecología y la conducción de grupos turísticos. La ecología estudia las interacciones entre los seres vivos y su entorno, abarcando niveles como especie, población, comunidad, bioma, biosfera y ecosistema. Los recursos naturales, esenciales para la vida, son afectados por la contaminación del aire, agua y suelo, lo que provoca desequilibrios ecológicos. Las áreas naturales se clasifican en protegidas públicas y privadas, con el objetivo de preservar la biodiversidad y garantizar el equilibrio ambiental. En los recorridos por la naturaleza, se enfatiza la importancia de proteger los ecosistemas y recursos naturales, vitales para la supervivencia de todas las especies.

    .row.justify-content-center
      .col-lg-12.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="En la síntesis de este componente se puede detallar temas como ecología y conducción de grupos turísticos, ecología y recursos naturales, historia y geografía turística, legislación ambiental, filosofía e historia, fundamentación científica y metodología 'No deje rastro'.")
      .col-auto
        a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
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
