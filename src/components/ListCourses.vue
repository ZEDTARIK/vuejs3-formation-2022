<template lang="">

    <div class="col-md-4" v-for="course in Courses" :key="course.id">
            <OneCourse :course="course" @deleted="onDelete($event)" />
    </div>

</template>
<script>
    
    import OneCourse from './OneCours.vue'
    
    export default {
        components: {
            OneCourse,
        },
        data() {
            return {
                Courses: [{
                        id: 1,
                        title: 'Learn Angular',
                        image: 'https://process.fs.teachablecdn.com/ADNupMnWyR7kCWRvm76Laz/resize=width:705/https://www.filepicker.io/api/file/nrOHB2iQTIiGe7hHX9O0'
                    },
                    {
                        id: 2,
                        title: 'Learn JavaScript',
                        image: 'https://process.fs.teachablecdn.com/ADNupMnWyR7kCWRvm76Laz/resize=width:705/https://www.filepicker.io/api/file/H9QyEOsSLG05qNb2kC0V'
                    },
                    {
                        id: 3,
                        title: 'Learn Git/Github',
                        image: 'https://process.fs.teachablecdn.com/ADNupMnWyR7kCWRvm76Laz/resize=width:705/https://www.filepicker.io/api/file/evNSVH9RSjW0um2vBYW9'
                    }

                ]
            }
        },
        methods: {
            onDelete(id) {
                this.Courses = this.Courses.filter(course => course.id != id);
            }
        }
    }
</script>
<style Scoped>
h4 {
    color: green;
}
</style>