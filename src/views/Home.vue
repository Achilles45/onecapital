<template>
  <div class="home">
   <Banner />
   <Partner />
   <About />
   <Investments />
   <Why />
   <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue';
import Partner from '@/components/Partner.vue';
import About from '@/components/About.vue';
import Investments from '@/components/Investments.vue';
import Why from '@/components/Why.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'home',
  components:{
    Banner,
    Partner,
    About,
    Investments,
    Why,
    Footer
  }
}
</script>
