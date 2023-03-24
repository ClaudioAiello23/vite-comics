<!-- PARTE VUE JS-->
<script>
import AppHeader from './components/AppHeader.vue';  // import dei files dalla cartella components
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components: {
    AppHeader, // aggiunta files dall'oggetto components 
    AppMain,
    AppFooter,
  }
}
</script>

<!-- PARTE HTML -->
<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

