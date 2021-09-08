<template>
  <div>
    <section id="nosotros">
      <b-row class="contenedor-cards">
        <b-col cols="12" class="card-1">
          <h1>17 años de experiendia en pos de tu proyecto</h1>
          <p>Especializados desde 1996 en usbilidad, experiencia de usuario (UX) y diseño de experiencia de proyectos digitales. Aportamos estrategia e innovacion centrada en el usuario y los objetivos de negocio de tu proyecto. Cotrabajando mejoramos tu tasa de conversion, KPI's, ROI y los resultados de tu actual publicidad PPC (pay per click)</p>
        </b-col>
        <b-col md="4" class="card-2">
          <h3>Estrategia, usabilidad & ux</h3>
          <p>Te ofrecemos excelente usabilidad y experiencia del usuario en tu proyeecto, junto a una cisión innovadora</p>
        </b-col>
        <b-col md="4" class="card-3">
          <h3>Mejora la experiencia</h3>
          <p>Tangibilizamos tu proyecto digital a través de un diseño centrado en el usuario y técnicas avanzadas</p>
        </b-col>
        <b-col md="4" class="card-4">
          <h3>Medición continua de objetivos</h3>
          <p>Implementación testing con usuarios y medición continua son necesarias para garantizar el éxito de tu proyecto</p>
        </b-col>
      </b-row>
    </section>
  </div>
</template>
<style lang="scss">
  .contenedor-cards {
    font-family: 'Graphik', sans-serif;
    .card-1 {
      background-color: #273138;
      text-align: center;
      padding: 40px;
      h1 {
        color: white;
        margin-bottom: 30px;
        padding-bottom: 20px;
        position: relative;
        &::after {
          content: "";
          position: absolute;
          display: block;
          width: 80px;
          height: 3px;
          bottom: 0;
          background: #00be0f;
          left: calc(50% - 40px);
        }
      }
      p {
        color: white;
        margin-bottom: unset;
      }
      @media (min-width: 992px) {
        padding: 80px 240px 60px 240px;
        p {
          padding-left: 60px;
          padding-right: 60px;
        }
      }
    }
    .card-2 {
      background-color: #3b4148;
    }
    .card-3 {
      background-color: #161c21;
    }
    .card-4 {
      background-color: #202a37;
    }
    .card-2, .card-3, .card-4 {
      text-align: center;
      padding: 40px;
      h3 {
        font-weight: 400;
        color: #00be0f;
      }
      p {
        color: white;
        margin-bottom: unset;
      }
      @media (min-width: 992px) {
        padding: 100px 80px 100px 80px;
        p {
          padding-left: 50px;
          padding-right: 50px;
        }
      }
    }
  }
</style>
