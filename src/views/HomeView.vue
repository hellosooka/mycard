<script>
import TheAbout from '../components/TheAbout.vue'
import TheSerivce from '../components/TheSerivce.vue'
import TheContacts from '../components/TheContacts.vue'


export default {
  components: {
    'the-about': TheAbout,
    'the-service': TheSerivce,
    'the-contacts': TheContacts,
    
  }
}

</script>

<template>
  <main>
    <the-about> </the-about>
    <the-service> </the-service>

    
    <the-contacts> </the-contacts>

  </main>
</template>
