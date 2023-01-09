<template>
    <div class="bounding-box">
        <p class="subtitle">
            {{ name }}
        </p>
        <slot name="icon"></slot>

    </div>
</template>
<script>
export default {
    props: ['name'],
    components: {

    },
    data() {
        return {

        }
    },

}
</script>
<style scoped>

</style>