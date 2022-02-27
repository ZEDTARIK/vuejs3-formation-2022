<template lang="">

    <div class="col-md-4" v-for="course in Courses" :key="course.id">
        <div class="card">
            <img class="card-img-top" :src="course.image" :alt="course.title">
            <div class="card-body">
                <h4 class="card-title"> {{ course.title }} </h4>
                <p class="card-text">
                    Lorem ipsum dolor sit amet consectetur...
                </p>
            </div>
        </div>
    </div>

</template>
<script>
    export default {
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
        }
    }
</script>
<style Scoped>
h4 {
    color: green;
}
</style>