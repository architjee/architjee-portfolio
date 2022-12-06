
<template>
    <span>
        <Ability :key="display" :mability="display" @fullyrendered="display_next()" class="has-text-weight-bold"></Ability>
</span>
</template>

<script>
import Ability from './Ability.vue';

export default {
    props: ["abilities"],
    data() {
        return {
            display: this.abilities[0],
            iter_index: -1,
            mainInterval: 0
        };
    },
    methods: {
        display_next() {
            
            if (this.iter_index < this.abilities.length - 1) {
                this.iter_index += 1;
                this.display = this.abilities[this.iter_index];
            }
            else {
                this.iter_index = 0;
                this.display = this.abilities[0];
                
            }
        },
    },
    mounted() {
        this.display_next()
    },
    components: { Ability }
}
</script>