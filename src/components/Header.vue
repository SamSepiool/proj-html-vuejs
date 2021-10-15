<template>
  <header class="w-100 position-fixed">
    <div class="container-fluid">
        <div class="row align-items-center px-5 py-3">

            <div class="col-lg-10">
                <div class="logo">
                    <img class="w-100" src="../assets/img/avada-music-logo-retina.png" alt="" />
                </div>
            </div>
            <div class="col-lg-2 text-end">
                <span @click='openMenu = !openMenu'> <font-awesome-icon class="fs-3 text-white" :icon='openMenuIcon'/> </span>
            </div>
            
            <transition name="menu">
              <nav v-if="openMenu">

                <div class="text-end p-5">
                  <span @click='openMenu = !openMenu'> <font-awesome-icon class="fs-2 text-white" :icon='closeMenuIcon'/> </span>
                </div>

                <ul class="d-flex flex-column justify-content-evenly text-center">
                  <li v-for="(link, index) in links" :key="index"><a class="fs-2" :href="link.url">{{link.name}}</a></li>
                </ul>
              </nav>
            </transition>
            
            
        </div>
    </div>
    
  </header>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faBars as faBars } from '@fortawesome/free-solid-svg-icons';
import { faTimes as faTimes } from '@fortawesome/free-solid-svg-icons';



export default {
  name: "Header",
  props: {
    links: Array,
  },
  components: {
      FontAwesomeIcon,
  },
  data(){
    return{
        openMenuIcon: faBars,
        closeMenuIcon: faTimes,

        openMenu: false,
    }
  },
  methods: {},
};
</script>

<style lang='scss' scoped>
@import "../assets/style/variables.scss";

header {
background-color: transparent;

  .logo {
    width: 20rem;
  }
  
  
  // MENU-OPEN
  nav{
    width: 100vw;
    height: 100vh;
    position: absolute;
    top: 0;
    left: 0;
    background-color: $primaryRed;

    ul{
      height: 80%;

      a{
        text-decoration: none;
        color: $menuLinks;

        &:hover{
          color: $white;
        }
      }
    }
  }
  // MENU-TRANSITION
  .menu-enter-active, .menu-leave-active {
    transition: opacity .8s ease-out;
  }
  .menu-enter, .menu-leave-to{
    opacity: 0;
  }
}
</style>