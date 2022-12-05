<template>
    {{ display }}
</template>

<script>
export default {
    props: ['abilities'],
    data() {
        return {
            display: this.abilities[0],
            iter_index: -1,
        }
    },
    methods: {
        display_next() {
            if (this.iter_index < this.abilities.length-1) {
                this.iter_index += 1
                this.display = this.abilities[this.iter_index];
            }else{
                this.iter_index = 0
                this.display = this.abilities[0]
            }
        },
    },
    mounted() {
        setInterval(this.display_next, 1000);
    }
}
</script>