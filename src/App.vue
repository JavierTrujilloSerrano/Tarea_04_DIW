<template>
  <Cabecera />
  <Menu />
  <div class="juntar">
  <Main />
  <Descripcion />
  <Pie />
  </div>
</template>

<script>
import Cabecera from './components/cabecera.vue'
import Menu from './components/menu.vue'
import Main from './components/main.vue'
import Descripcion from './components/descripcion.vue'
import Pie from './components/pie.vue'

export default {
  name: 'App',
  components: {
    Cabecera,
    Menu,
    Main,
    Descripcion,
    Pie
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.juntar{
  display:flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin: 1rem;
  justify-content: center;
}
</style>
