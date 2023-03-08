<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  
  <div class="greetings">
    <h1 class="green">{{ msg }}
      Laboratorio de sistemas y aplicaciones web
    </h1>
    <h1>  
      <img src="http://isclab.com.mx/img/svg/email.svg" width="20" height="20"> email contacto@isclab.com.mx
    </h1>
  </div>
  <br>
  <div>
    <h2>
        ¿Qué hacemos en isclab?
    </h2>
    <h4>
        Desarrollamos aplicaciones con fines de práctica, investigación y responsabilidad social.
        Buscamos el desarrollo de nuestros estudiantes a través de la creación de proyectos que sean útiles a la sociedad.
        ¿Tienes un proyecto en mente? Compártelo con nosotros y buscaremos la manera de ayudarte.
    </h4>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
