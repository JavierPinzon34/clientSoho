<template>
  <section id="footer">
    <div class="contenedor">
      <b-row class="contenido-footer">
        <b-col md="4" class="contenido-copy">
          <h5><strong>&copy; 2017</strong> SOHO internet + humana</h5>
        </b-col>
        <b-col md="4" class="contenido-links">
          <a href="">Visítanos</a>
          <a href="">Escríbenos</a>
          <a href="">Llámanos</a>
        </b-col>
        <b-col md="4" class="contenido-redes">
          <a href="" class="facebook">Facebook</a>
          <a href="" class="twitter">Twitter</a>
          <a href="" class="linkedin">Linkedin</a>
          <a href="" class="youtube">Youtube</a>
        </b-col>
      </b-row>
    </div>
  </section>
</template>
<style lang="scss">
  .contenido-footer {
    font-family: 'Graphik', sans-serif;
    background-color: black;
    padding: 30px;
    .contenido-copy {
      color: white;
      h5 {
        font-weight: 300;
        margin: 0;
        strong {
          color: white;
          font-weight: bold;
        }
      }
      @media (max-width: 991.98px) {
        text-align: center;
        margin-bottom: 5px;
      }
    }
    .contenido-links {
      text-align: center;
      a {
        color: #00be0f;
        margin-left: 20px;
        margin-right: 20px;
        @media (max-width: 991.98px) {
          margin: 6px;
        }
      }
      @media (max-width: 991.98px) {
        margin-bottom: 5px;
      }
    }
    .contenido-redes {
      text-align: right;
      a {
        margin-left: 15px;
        margin-right: 15px;
        @media (max-width: 991.98px) {
          margin: 5px;
        }
      }
      .facebook {
        color: #4658bc;
      }
      .twitter {
        color: #0ad2ff;
      }
      .linkedin {
        color: #4a90e2;
      }
      .youtube {
        color: #eb6f6f;
      }
      @media (max-width: 991.98px) {
        text-align: center;
      }
    }
    @media (max-width: 991.98px) {
        padding: 10px;
    }
  }
</style>
