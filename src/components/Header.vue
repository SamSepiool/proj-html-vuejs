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
                <a> <font-awesome-icon class="fs-3 text-white" :icon='menuIcon'/> </a>
            </div>
        </div>
    </div>
    
  </header>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faBars as faBars } from '@fortawesome/free-solid-svg-icons';

export default {
  name: "Header",
  props: {},
  components: {
      FontAwesomeIcon,
  },
  data(){
    return{
        menuIcon: faBars
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
}
</style>