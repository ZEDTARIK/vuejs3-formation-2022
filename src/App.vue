<template>
  <div class="container">
    <div class="row my-3">
      <div class="col-md-12">
        <Header></Header>
      </div>
    </div>

    <Employee />
    
    <Footer author="Zouhair ETTARAK" Year="@ 2022"></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Employee from "./components/employee/Employee.vue"

export default {
  name: "App",
  components: {
    Header,
    Footer,
    Employee,
  }
};
</script>

<style>
</style>
