<script >
import Abilities from '../components/Abilities.vue';
import Ability from '../components/Ability.vue';
export default {
  components: {
    Abilities,
    Ability
  },
  data() {
    return {
      abilities_const: ['a Data Science Enthusiast,', 'a Software Developer,', 'working with Web Technologies,', 'also sometimes doing Game development too.']
    }
  },
  methods:{
    
  }
}
</script>

<template>
  <div>
  
  <p class="title">
   <span class="has-text-grey">

     I am 
    </span>
    <Abilities :abilities="abilities_const" class="has-text-dark	"></Abilities>
  </p>
 
  </div>
</template>
