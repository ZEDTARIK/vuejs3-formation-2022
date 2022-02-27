<template>
  <div class="container">
    <div class="row my-3">
      <div class="col-md-12">
        <Header></Header>
      </div>
    </div>

    <div class="row">
      <div class="col-md-6 mx-auto">
        <AddCours />
      </div>
    </div>

    <div class="row my-2">
      <ListCourses />
    </div>

    <Footer author="Zouhair ETTARAK" Year="@ 2022"></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import AddCours from "./components/AddCours.vue";
import ListCourses from "./components/ListCourses.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    AddCours,
    ListCourses,
    Footer,
  },
  data() {
    return {
      message: "Lorem ipsom",
    };
  },
};
</script>

<style>
</style>
