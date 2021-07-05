<template>
  <div>
    <div class="banner dark-overlay" style="background-image: url('/img/banner/1.jpg')">
      <div class="container">
            <VueSlickCarousel v-bind="settings">
              <div class="">
                <div class="banner-inner">
                  <h1 class="title text-white">Getting Education Became   <span class="custom-primary">Easier</span> </h1>
                  <p class="subtitle text-white">Bacon ipsum dolor amet ball tip pork chop cow tenderloin andouille. Pastrami pork picanha tongue venison strip steak</p>
                  <a href="#" class="btn-custom primary shadow-none">Access 100 Books Now <font-awesome-icon :icon="['fa', 'arrow-right']" :style="{ marginLeft: '10px' }"/> </a>
                </div>
              </div>
              <div class="">
                <div class="banner-inner">
                  <h1 class="title text-white">Learn The <span class="custom-primary">Physics</span>Play With Physics</h1>
                  <p class="subtitle text-white">Bacon ipsum dolor amet ball tip pork chop cow tenderloin andouille. Pastrami pork picanha tongue venison strip steak</p>
                  <a href="#" class="btn-custom primary shadow-none">Contact Me <font-awesome-icon :icon="['fa', 'arrow-right']" :style="{ marginLeft: '10px' }"/></a>
                </div>
              </div>
              <div class="">
                <div class="banner-inner">
                  <h1 class="title text-white"><span class="custom-primary">Elevate</span>Communication Skill In English </h1>
                  <p class="subtitle text-white">Bacon ipsum dolor amet ball tip pork chop cow tenderloin andouille. Pastrami pork picanha tongue venison strip steak</p>
                  <a href="#" class="btn-custom primary shadow-none">Visit My Blog <font-awesome-icon :icon="['fa', 'arrow-right']" :style="{ marginLeft: '10px' }"/></a>
                </div>
              </div>
            </VueSlickCarousel>
      </div>
    </div>
  </div>
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
  export default {
    components:{
      VueSlickCarousel,
    },
    data(){
      return {
        settings: {
          arrows: true,
          dots: false,
          slidesToShow: 1,
          slidesToScroll: 1,
        }
      }
    }
  }
</script>

<style>
  .abc{
    text-decoration: none;
  }

  .slick-prev {
    left: -74px;
  }

  .slick-next {
    right: -74px;
  }

</style>
