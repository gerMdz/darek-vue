<script lang="ts" >
import { defineComponent }from 'vue'
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'

export default defineComponent({
  name: 'App',
  components: {
    HelloWorld,
    TheWelcome
  }
})
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="
      <p>Estás aquí. <br/>Vue y TS</p>" />
    </div>
  </header>


  <main>
    <h1>Desde aquí</h1>
    <TheWelcome />
  </main>
</template>

<style>
header {
  line-height: 1.5;
}

h4 {
  color: #2c3e50;
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
