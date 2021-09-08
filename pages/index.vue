<template>
  <div class="container-fluid contenedor-index">
    <NavBar/>
    <Inicio/>
    <Banner/>
    <Nosotros/>
    <Proyecto/>
    <Footer/>
    <div class="icono-plus">
        <img src="@/assets/img/plus.svg" alt="">
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
  .contenedor-index {
    padding: unset;
    height: 100vh;
    .icono-plus {
      text-align: center;
      width: 100%;
      z-index: 99999;
      position: relative;
      top: -124px;
      right: 0;
      @media (max-width: 767.98px) {
        top: -139px;
      }
    }
  }
  .row {
    margin: 0;
  }
</style>
