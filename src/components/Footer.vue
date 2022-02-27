<template lang="">
    <div class="row my-5">
        <div class="col-md-12 text-center">
                <span>
                    {{ author }}  {{ Year }}
                </span>
        </div>
    </div>
</template>
<script>
    export default {
        props: ['author', 'Year' ]
    }
</script>
<style lang="">

</style>