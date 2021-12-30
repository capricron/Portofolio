<template>
  <div class="konten">
     <div id="nav">
       <Navbar />
    </div>
  </div>

  <router-view/>
</template>

<script>
  import Navbar from '@/components/Nav.vue';
  export default{
    components:{
      Navbar
    }
  }
</script>


<style>

  .konten{
    color: white;
  }
</style>