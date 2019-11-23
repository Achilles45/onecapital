<template>
  <div class="home">
   <Banner />
   <Partner />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue';
import Partner from '@/components/Partner.vue';

export default {
  name: 'home',
  components:{
    Banner,
    Partner
  }
}
</script>
