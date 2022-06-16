<script>
import TheHeader from './components/TheHeader.vue'

export default {

  components: {
    'the-header': TheHeader
  }
}
</script>

<template>
  <the-header> </the-header>

  <router-view/>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;600;700&display=swap');

#app {
  font-family: Rubik;
}

*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

</style>
