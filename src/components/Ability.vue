<template>
  <span>
      {{ display }}
  </span> 
</template>

<script>
export default {
    props: ['mability'],
    data() {
        return {
            display: this.mability[0],
            iter_index: 0,
            is_caret : false,
        }
    },
    methods: {
        display_next() {
            if (this.iter_index < this.mability.length) {
                this.is_caret = !this.is_caret;
                this.iter_index += 1
                this.display = this.mability.substring(0,this.iter_index) + (this.is_caret?'_':'');
            }else{
                this.$emit('fullyrendered')
            }
        },
    },
    mounted() {
        this.mainInterval = setInterval(this.display_next, 120);
    }
}
</script>