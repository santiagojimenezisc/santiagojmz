<template>
  <div id="aplicacion" class="container">
     <Header></Header>
     <Footer></Footer>
  <router-view />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

export default {
  name:"aplicacion",
    components: {
    Header,
    Footer,
  },
}
</script>
<style>
#app {
  font-family: 'Poppins';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: #FCFDFF;
  overflow-x: hidden;
}
</style>
