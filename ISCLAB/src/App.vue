<script setup>
import Titulo from './components/Titulo.vue'
import Pregunta from './components/Pregunta.vue'
import Pregunta2 from './components/Pregunta2.vue'
import Pregunta3 from './components/Pregunta3.vue'
import Piepag from './components/PiePag.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <Titulo msg="" />
    </div>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="600" height="300" />
  </header>
  <br>
  <br>
  <main>
    <Pregunta />
    <br>
    <Pregunta2 />
    <br>
    <Pregunta3 />    
  </main>
  <br>
  <br>
  <footer>
    <Piepag /> 
  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    background-color: #40E0D0;
  }
  footer{
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    background-color: #40E0D0;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
