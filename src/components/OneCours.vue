<template lang="">
       <div class="card">
            <img class="card-img-top" :src="course.image" :alt="course.title">
            <div class="card-body">
                <h4 class="card-title"> {{ course.title }} </h4>
                <p class="card-text">
                    Lorem ipsum dolor sit amet consectetur...
                </p>
            </div>

            <div class="card-footer">
                <button class="btn btn-danger btn-sm" type="button" @click="deleteCourse(course.id)">Delete</button>
            </div>
        </div>
</template>
<script>
export default {
    props: ["course"],
    methods: {
        deleteCourse(id) {
            this.$emit('deleted', id);
        }
    },
}
</script>
<style lang="">
    
</style>