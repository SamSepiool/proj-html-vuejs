<template>
  <div id="app">

    <Header/>
    <Main/>
    <Footer :links="footerLinks" />

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'





export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  },
  data(){
    return{
      footerLinks:[
        {
          name: 'Home',
          url: '#'
        },
        {
          name: 'Meet the Band',
          url: '#'
        },
        {
          name: 'Live Dates',
          url: '#'
        },
        {
          name: 'Latest News',
          url: '#'
        },
        {
          name: 'Albums',
          url: '#'
        },
        {
          name: 'Fans',
          url: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';

</style>
