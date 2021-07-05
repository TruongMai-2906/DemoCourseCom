

<template>
  <div>
    <Banner />
    <Categories />
    <About />
    <Services />
  </div>
</template>

<script lang='ts'>
  import Vue from "vue";
  import Banner from "~/components/Banner.vue"
  import Categories from "~/components/Categories.vue"
  import About from "~/components/About.vue"
  import Services from "~/components/Services.vue"
  export default Vue.extend({
    components: {
      Banner,
      Categories,
      About,
      Services
    },
    layout: 'default',
  })
</script>



