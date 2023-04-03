
<template>
  <div class="formulario">
  <form action="">
    <div>
<p>DIGITE SEU NOME:</p>
<input v-model="nome" placeholder="DIGITE SEU NOME"/>

<p>DIGITE SEU EMAIL:</p>
<input v-model="email" placeholder="DIGITE SEU EMAIL"/>

  </div>
  </form>
</div>



</template>

<script setup>
import { ref } from 'vue'

const nome = ref('')
</script>


<style scoped>
.formulario{
background-color: rgb(255, 0, 51);
border: 8px solid black;
color: black;
font-family: 'Times New Roman', Times, serif;

}

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
