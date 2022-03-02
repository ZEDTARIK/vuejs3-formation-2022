<template lang="">
    <div class="row"  >
        <div class="col-md-6 mx-auto" v-if="showForm">
            <AddCours />
        </div>
    </div>
    <div class="row mt-2">
        <div class="col-md-12 text-right">
            <button class="btn btn-success btn-sm" type="button" @click="displayForm">New</button>
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
    },
    data() {
        return {
            showForm: false,
        }
    },
    methods: {
        displayForm() {
            this.showForm = !this.showForm;
        }
    },
}
</script>
<style lang="">
    
</style>