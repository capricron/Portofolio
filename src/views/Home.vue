<template>
  <link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css" integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous"/>
  
  <div class="container konten home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <Biodata />
    <div class="row">
      <div class="col-lg-5">
        <Pendidikan/>
      </div>
      <br>
      <div class="col-lg-2 center">
        <div class="garis"></div>
      </div>
      <br>
      <div class="col-lg-5">
        <Pengalaman/>
      </div>
    </div>
      <Alat/>
    <br>
  </div>
      <Footer/>
</template>

<script>
// @ is an alias to /src

import 'bootstrap/dist/css/bootstrap.min.css'
import 'bootstrap/dist/js/bootstrap.min.js'

import Biodata from '../components/home/Biodata.vue';
import Pendidikan from '../components/home/Pendidikan.vue';
import Pengalaman from '../components/home/Pengalaman.vue';
import Alat from '../components/home/Alat.vue';
import Footer from '../components/home/Footer.vue';

export default {
  name: 'Home',
  components: {
    Biodata,
    Pendidikan,
    Pengalaman,
    Alat,
    Footer
  }
}
</script>
<style>
  body{
    background: black;
  }



  .garis{
    margin-left: 50px;
    width: 10%;
    margin-top: -70px;
    height: 150%;
    background-color: white;
  }

    .footer{
        height: 50px !important;
        width: 100% !important;
        background-color: #FFD700;
  }

  @media (max-width:1000px) {
    .garis{
      display: none;
    }

    .pengalaman h1, .pendidikan h1{
      font-size: 35px;
    }

    .pengalaman{
      margin-top: 50px;
    }
  }
</style>

