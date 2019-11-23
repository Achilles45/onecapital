<template>
  <div class="home">
   <Banner />
   <Partner />
   <About />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue';
import Partner from '@/components/Partner.vue';
import About from '@/components/About.vue';

export default {
  name: 'home',
  components:{
    Banner,
    Partner,
    About
  }
}
</script>
