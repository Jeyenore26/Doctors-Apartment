<template >
  <main class="gradient">
      <section class="lg:mx-[8rem] mx-4 ">
          <NavBar/>
          <Homepage/>
      </section>
  </main>

</template>

<script>
import Homepage from './components/Homepage.vue';

import NavBar from './components/NavBar.vue';

export default {
  components:{
      Homepage,

      NavBar,
  }
};
</script>

<style>
.gradient{
  background-image: linear-gradient(to right , #d4fbff , #e1fcff,  #fff , #e1fcff , #d4fbff);
  height: 100%;
  width: 100%;
}
</style>