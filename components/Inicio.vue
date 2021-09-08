<template>
  <div class="container-fluid home-page">
    <section id="inicio" >
      <div class="contenido-inicio">
        <div class="texto">
          <h1 class="titulo-1">
            Nos especializamos en
          </h1>
          <h1 class="titulo-2">
            interfaces digitales que los usuarios aman
          </h1>
          <div class="text-center">
            <a ref="#">HABLEMOS DE TU PROYECTO</a>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<style lang="scss">
  .home-page {
    font-family: 'Graphik', sans-serif;
    height: 100vh;
    background: url('../assets/img/space.jpg') no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    .contenido-inicio {
      display: flex;
      align-content: center;
      align-items: center;
      justify-content: center;
      min-width: 100%;
      height: 100vh;
      .texto {
        .titulo-1 {
          color: white;
          @media (min-width: 576px) {
            font-size: 50px;
          }
          font-weight: 400;
          text-align: center;
          margin-bottom: 0;
        }
        .titulo-2 {
          color: #00be0f;
          @media (min-width: 576px) {
            font-size: 60px;
          }
          font-weight: 600;
          text-align: center;
          margin-bottom: 60px;
        }
        a {
          background-color: #00be0f;
          padding: 20px 50px 20px 50px;
          color: white;
          border-radius: 5px;
          width: 350px;
          height: 70px;
          font-weight: 500;
          border: unset;
          &:hover {
            background-color: #00be0f00;
            border: 1px solid white;
          }
          &:active {
            background-color: #00be0f;
          }
        }
      }
    }
  }
</style>
