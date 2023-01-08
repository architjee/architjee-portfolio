<script >
import Navbar from '../components/Navbar.vue';

export default {
  components: {
    Navbar
  },
  data() {
    return {
    }
  },
  methods: {

  }
}
</script>

<template>

  <section class="hero  is-fullheight">
    <div class="hero-head">
      <Navbar></Navbar>
    </div>
    <div class="hero-body">
      <div class="container has-text-centered">
        <p class="title">
          Title
        </p>
        <p class="subtitle">
          Subtitle
        </p>
      </div>
    </div>
  </section>

</template>
