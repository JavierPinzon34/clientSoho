<template>
  <header id="header">
    <div class="mi-navbar">
      <b-navbar toggleable="lg" type="dark" :class="`${scrollPosition > 50 ? 'header-scrolled' : ''}`">
        <img src="@/assets/img/logo.png" alt="">

        <b-navbar-toggle
          target="nav-collapse"
        />

        <b-collapse id="nav-collapse" is-nav>
          <!-- items alineados a la izquierda -->
          <b-navbar-nav class="ml-auto">
            <nuxt-link :to="{ path: '/',hash:'#inicio' }">
              inicio
            </nuxt-link>
            <nuxt-link :to="{ path: '/',hash:'#nosotros' }">
              nosotros
            </nuxt-link>
            <nuxt-link :to="{ path: '/',hash:'#servicios' }">
              servicios
            </nuxt-link>
            <nuxt-link :to="{ path: '/',hash:'#casos' }">
              casos de éxito
            </nuxt-link>
            <nuxt-link :to="{ path: '/',hash:'#equipo' }">
              únete al equipo
            </nuxt-link>
            <nuxt-link :to="{ path: '/',hash:'#footer' }">
              contacto
            </nuxt-link>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </header>
</template>
<script>
export default {
  data() {
    return {
      scrollPosition: null
    }
  },
  mounted () {
    window.addEventListener('scroll', this.updateScroll)
    window.onresize = () => {
      this.width = window.innerWidth
    }
  },
  destroy () {
    window.removeEventListener('scroll', this.updateScroll)
  },
  methods: {
    updateScroll () {
      this.scrollPosition = window.scrollY
    }
  },
}
</script>
<style lang="scss">
  .mi-navbar {
    font-family: 'Graphik', sans-serif;
    position: fixed;
    z-index: 100;
    width: 100%;
    .navbar-dark {
      padding: 15px 20px 15px 20px;
      background-color: transparent;
      transition: all .5s;
      a {
        color: rgb(255 255 255 / 65%);
        font-size: 20px;
        margin-left: 20px;
        margin-right: 20px;
        padding: unset;
        border-bottom: 3px solid #00be0f00;
        @media (min-width: 992px) {
          &:hover {
            color: white;
            border-bottom: 3px solid #00be0f;
            text-decoration: none;
          }
        }
      }
      .nuxt-link-active {
        @media (min-width: 992px) {
          border-bottom: 3px solid #00be0f;
          color: white;
        }
      }
      img {
        max-height: 80px;
        transition: all .5s;
      }
    }
    .header-scrolled {
      background-color: rgb(21 34 43 / 74%);
      img {
        transition: all .5s;
        max-height: 40px;
      }
    }
  }


</style>
