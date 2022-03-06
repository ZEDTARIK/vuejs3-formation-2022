<template>
  <div class="container">
    <div class="row my-3">
      <div class="col-md-12">
        <Header></Header>
      </div>
    </div>

    <Course />
    
    <Footer author="Zouhair ETTARAK" Year="@ 2022"></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Course from "./components/course/Course.vue"

export default {
  name: "App",
  components: {
    Header,
    Footer,
    Course,
  }
};
</script>

<style>
</style>
