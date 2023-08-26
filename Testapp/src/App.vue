<script setup>

import TheWelcome from './components/TheWelcome.vue'
import Home from './components/Home.vue'
import Products from './components/Products.vue'
import Counter from './components/Counter.vue'
import Reactive from './components/Reactive.vue'

</script>

<template>
 
  <main>
      <Home  title="Done by Rohullah Kyhan " msg="Hello, world today I have my first job   interview they encourge me to start vue js "/>
      <br>
    
      <Reactive  title="Reactive Component" />
  </main>
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
