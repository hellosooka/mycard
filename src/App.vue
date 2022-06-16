<script>
import TheHeader from './components/TheHeader.vue'
import TheAbout from './components/TheAbout.vue'

export default {

  components: {
    'the-header': TheHeader,
    'the-about': TheAbout,
  }
}
</script>

<template>
  <div class="wrapper">
    <the-header> </the-header>
    <the-about> </the-about>


    <router-view/>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;600;700&display=swap');

.wrapper {
  min-height: 100%;
  overflow: hidden;
}


#app {
  font-family: Rubik;
  
}

*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

</style>
