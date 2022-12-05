<script >
import Abilities from '../components/Abilities.vue';
export default {
  components: {
    Abilities
  },
  data() {
    return {
      abilities_const: ['ML based classification','Web Development','Wireframing','and sometimes Game dev. too']
    }
  }
}
</script>

<template>
I can do <Abilities :abilities="abilities_const"></Abilities>
</template>
