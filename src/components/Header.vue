<template>
  <header>
      <div class="logo">
          <img src="../assets/img/avada-music-logo-retina.png" alt="">
      </div>


      <button id="open" @click='openMenu()' >
          menu
      </button>

      
    <!-- <nav id="overlay_menu" class="menu">

      <button id="close" @click='closeMenu()' >chiudi</button>

      <ul class="voices">
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
      </ul>

  </nav> -->
      

    

  </header>
</template>

<script>

export default {
    name: 'Header',
    components:{
       
    },
    props:{

    },
    methods:{
       
        
    }

}
</script>

<style lang='scss' scoped>
@import '../assets/style/variables.scss';

header{
    background-color: transparent;
    padding: .75rem 3.125rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: fixed;
    width: 100%;


    .logo{
        width: 20rem;
        img{
            width: 100%;
        }
    }
  
    
  

   
}
    

   


</style>