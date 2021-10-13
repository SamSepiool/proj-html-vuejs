<template>
  <main>
      <section class="hero text-white">

          <div class="container-fluid h-100">
              <div class="row h-100 text-center align-items-center" >
                  <div class="col">
                      <h1 class="fw-bold"> Untold Stories </h1>
                      <p class="fs-3">There is an untold story behind every favorite song.</p>
                      <div class="buttons ">
                        <button type="button" class="fw-bold mx-3 px-5 py-3 btn btn-secondary">LATEST ALBUM</button>
                        <button type="button" class="fw-bold mx-3 px-5 py-3 btn btn-outline-secondary">LIVE DATES</button>
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
                    <hr class="mx-auto mb-4">
                    <div class="box">
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ipsa dolores rerum nostrum quam reiciendis voluptatem error animi, maiores adipisci sapiente vero magnam qui ut. Earum est totam ipsa impedit?</p>
                    </div>    
                </div>
                    
            </div>
        </div>
          
      </section>

  </main>
</template>

<script>
export default {
    name:'Main',
    components:{

    }
}
</script>

<style lang='scss' scoped>
@import '../assets/style/variables.scss';
// .row{
//     border: 1px solid blue;
// }
.hero{
    background-image: url(../assets/img/home_slider.jpg);
    background-size: cover;
    background-position:bottom;
    height: 100vh;
    
    h1{
        font-size: 9.375rem !important;
    }

    .buttons{
        

        & button:first-child{
            background-color:$primaryRed;
            border: none;
        }
        & button:last-child{
            border-color: white;
            color: white;
        }

        button:hover{
            background-color: white;
            color: black;
        }
    }
  
    
}

.is_life{
    background-color: $primaryGray;

    .bookmark{
        background-color: $primaryRed;
        height: .75rem;
        width: 40%;
    }
}

</style>