<template>
    <div class="single-progress">
        <div class="is-size-5">
            {{ label }}
        </div>
        <progress class="progress" :value="size" max="100" :class="color">{{size}}</progress>
    </div>
</template>
  
<script>
export default {
    props: ['label','size','color'],
    data() {
        return {

        }
    },
    methods: {

    },
    mounted() {

    }
}
</script>