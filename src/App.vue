<template>
  <div id="app">

    <Header/>
    <Main/>

    <main>
      <!-- SECTION  untold stories-->
      <!-- SECTION music is life-->

      <section> <!-- latest brand news -->
        <!-- CARD -->
      </section>

      <!-- SECTION review -->
      <!-- SECTION live dates -->
    </main>

    <footer>
      <!-- FOOTER-TOP -->
      <!-- FOOTER-BOTTOM -->
    </footer>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'




export default {
  name: 'App',
  components: {
    Header,
    Main
    
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';

</style>
