<template>
  <main>
    <section class="hero text-white">
      <div class="container-fluid h-100">
        <div class="row h-100 text-center align-items-center">
          <div class="col">
            <h1 class="fw-bold">Untold Stories</h1>
            <p class="fs-3">
              There is an untold story behind every favorite song.
            </p>
            <div class="buttons">
              <button
                type="button"
                class="fw-bold mx-3 px-5 py-3 btn btn-secondary"
              >
                LATEST ALBUM
              </button>
              <button
                type="button"
                class="fw-bold mx-3 px-5 py-3 btn btn-outline-secondary"
              >
                LIVE DATES
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="is_life">
      <div class="container text-white">
        <div class="row">
          <div class="col">
            <div class="bookmark mx-auto my-0"></div>
          </div>
        </div>

        <div class="row text-center py-5">
          <div class="col">
            <h2 class="fs-1 fw-bold">Music is Life</h2>
            <hr class="mx-auto mb-4" />
            <div class="box">
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ipsa
                dolores rerum nostrum quam reiciendis voluptatem error animi,
                maiores adipisci sapiente vero magnam qui ut. Earum est totam
                ipsa impedit?
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="latest_brand">
      <div class="container text-white">
        <div class="row text-center py-5">
          <div class="col">
            <h2 class="fs-1 fw-bold">Latest Brand News</h2>
            <hr class="mx-auto mb-4" />
            <div class="box">
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ipsa
                dolores rerum nostrum quam reiciendis voluptatem error animi,
                maiores adipisci sapiente vero magnam qui ut. Earum est totam
                ipsa impedit?
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="container py-5">
          
       <!-- PIANO CARDS -->
       <img class="w-100" src="http://www.tacchi.it/wp-content/uploads/2017/11/pp-work-in-progress-624x434.jpg" alt="">

      </div>
      <FullBtn/>
      
    </section>

    

    
  </main>
</template>

<script>
import FullBtn from './FullBtn.vue'
export default {
  name: "Main",
  components: {
      FullBtn,
  },
};
</script>

<style lang='scss' scoped>
@import "../assets/style/variables.scss";
// .row{
//     border: 1px solid blue;
// }
.container{
    border: 1px solid red;
}
.hero {
  background-image: url(../assets/img/home_slider.jpg);
  height: 100vh;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  h1 {
    font-size: 9.375rem !important;
  }

  .buttons {
    & button:first-child {
      background-color: $primaryRed;
      border: none;
    }
    & button:last-child {
      border-color: white;
      color: white;
    }

    button:hover {
      background-color: white;
      color: black;
    }
  }
}

.is_life {
  background-color: $primaryGray;

  .bookmark {
    background-color: $primaryRed;
    height: 0.75rem;
    width: 40%;
  }
}

.latest_brand {
  background-color: $secondaryGray;
}


</style>