<template>
  <div>
    <section id="servicios">
      <div class="contenido-titulo">
        <h1>Proyectos destacados</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
      </div>
      <ItemProyecto
        v-for="(project, index) in allProjects"
        :key="index"
        :color="project.color"
        :code="project.code"
        :image-position="project.image_position"
        :name="project.name"
        :description="project.description"
        :tags="project.tags"
        :theme="project.theme"
      />
    </section>
  </div>
</template>
<script>
import axios from 'axios'
export default {
  data() {
    return {
      allProjects: {}
    }
  },
  mounted() {
    this.getProject()
  },
  methods: {
    async getProject() {
      try {
        const res = await this.$axios.get('projects')
        this.allProjects = [...res.data]
      } catch {
        console.log('error')
      }
    }
  },
}
</script>
<style lang="scss">
  .contenido-titulo {
    font-family: 'Graphik', sans-serif;
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
      padding: 120px 240px 60px 240px;
      p {
        padding-left: 60px;
        padding-right: 60px;
      }
    }
  }
</style>
