<template lang="">
    <div class="row">
        <div class="col-md-6 mx-auto">
            <AddCours />
        </div>
        </div>

    <div class="row my-2">
      <ListCourses />
    </div>
</template>
<script>
import AddCours from "./AddCours.vue"
import ListCourses from "./ListCourses.vue"
export default {
    components: {
        AddCours,
        ListCourses
    }
}
</script>
<style lang="">
    
</style>