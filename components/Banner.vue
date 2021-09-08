<template>
  <div class="banner-content">
    <b-row class="banner-head">
      <b-col md="8" class="banner-text">
        <h5>
          <img src="@/assets/img/live.svg" alt=""><span> EN DIRECTO</span> -Soho está presente en el <span>DIGITALBANK MONTEVIDEO</span>. "Experiencia de Usuario" por Alvaro Añón (SEO de Soho).
        </h5>
      </b-col>
      <b-col md="4" class="links">
        <button class="link-solid">VER EVENTO</button>
        <button class="link-line">PRÓXIMOS EVENTOS</button>
      </b-col>
    </b-row>
  </div>
</template>
<style lang="scss">
  .banner-content {
    font-family: 'Graphik', sans-serif;
    background-color: black;
    text-align: center;
    padding: 20px 45px 20px 45px;
    .banner-head {
      .banner-text {
        padding-top: 7px;
        h5 {
          font-size: 18px;
          margin-top: 0.5rem;
          color: white;
          font-weight: 300;
          img {
            height: 40px;
          }
          span {
            font-weight: 600;
          }
        }
      }
      .links {
        .link-solid {
          background-color: #00be0f;
          padding: 13px 20px 15px 20px;
          color: white;
          border-radius: 5px;
          width: 150px;
          height: 50px;
          font-weight: 500;
          border: unset;
          margin: 10px;
          &:hover {
            background-color: #00be0f00;
            border: 1px solid white;
            text-decoration: none;
          }
          &:active {
            background-color: #00be0f;
          }
        }
        .link-line {
          background-color: #00be0f00;
          padding: 13px 20px 15px 20px;
          color: #00be0f;
          border-radius: 5px;
          width: 200px;
          height: 50px;
          font-weight: 500;
          border: 1px solid #00be0f;
          &:hover {
            background-color: #00be0f;
            border: unset;
            text-decoration: none;
            color: white;
          }
          &:active {
            background-color: #00be0f00;
          }
        }
      }
    }
    @media (min-width: 992px) {
      height: auto;
     }
  }
</style>
