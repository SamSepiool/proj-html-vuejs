<template>
    <footer>
        <div class="top w-100 p-5">
            <div class="container-fluid">
                <div class="row align-items-center">
                    <div class="col">
                        <div class="logo">
                            <img class="w-100" src="../assets/img/logo_footer.png" alt="">
                        </div>
                    </div>
                    <div class="col">
                        <ul class="d-flex justify-content-end">
                            <li v-for="(link, index) in links" :key="index" ><a :href="link.url">{{link.name}}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="bottom w-100 p-5">
            <div class="container-fluid">
                <div class="row align-items-center">
                    <div class="col-lg-8">
                        <p>© Copyright 2012 - 2021 | Avada Theme by <span>ThemeFusion</span> | All Rights Reserved | Powered by <span>WordPress</span></p>
                    </div>
                    <div class="col-lg-4">
                        <ul class="d-flex justify-content-end">
                            <li><a href="#"><font-awesome-icon :icon="fb" /></a></li>
                            <li><a href="#"><font-awesome-icon :icon="tw" /></a></li>
                            <li><a href="#"><font-awesome-icon :icon="ig" /></a></li>
                            <li><a href="#"><font-awesome-icon :icon="yt" /></a></li>
                        </ul>
                    </div>
                </div>
            </div>

        </div>
    </footer>

      

</template>

<script>
import { faFacebookF as facebook } from '@fortawesome/fontawesome-free-brands';
import { faInstagram as instagram } from '@fortawesome/fontawesome-free-brands';
import { faTwitter as twitter } from '@fortawesome/fontawesome-free-brands';
import { faYoutube as youtube } from '@fortawesome/fontawesome-free-brands';



import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';



export default {
    name: 'Footer',
    components:{
       FontAwesomeIcon
    },
    props:{
        links: Array
    },
    data(){
        return{
            fb: facebook,
            tw: twitter,
            ig: instagram,
            yt: youtube
        }
    },
    methods:{
       
        
    }

}
</script>

<style lang='scss' scoped>
@import '../assets/style/variables.scss';

footer{
color: $gray;

    li{
        margin: .625rem;
        a{
            text-decoration: none;

            &:hover{
                color:white;
            }
        }
    }

    .top{
    background-color: $footerTop;

    .logo{
        width: 18rem;
        
    }

    
        
    a{
        text-decoration: none;
        color:inherit
    }
    
   
}


.bottom{
    background-color: $footerBottom;

    span{
        color:$primaryRed;
    }

    
    ul{
        li{
            text-align: center;
            line-height: 2.5rem;            
            a{
                background-color: $secondaryGray;
                display: inline-block;
                height: 2.5rem;
                width: 2.5rem;
                color: inherit;
            }

           
        }
    }
    
}

}
   


</style>