<template>

  <main>
 
     <Example1 />
    <Example2 />
    <ExampleForm />

  </main>

</template>

<script setup lang="ts">


// not the coolest component names, but it makes sense for this demo

import Example1 from './components/Example1.vue';
import Example2 from './components/Example2.vue';
import ExampleForm from './components/ExampleForm.vue';



</script>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 100vh;
  width: 100vw;
  background: #fff;
  width: 100%;
  font-family: arial, sans-serif;
}
</style>


<style>

.container {
    display: flex;
    margin: 0 auto;
    padding: 1.5rem;
}

.container.limited-width {
    max-width: 85% ;
}

button svg {
  display: block;
  width: 1rem;
  height: 1rem;
}

button[aria-label="show/hide navigation"] {
  border: 0;
}

</style>