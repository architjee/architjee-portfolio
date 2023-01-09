<script >
import Navbar from '../components/Navbar.vue';
import Footer from '../components/Footer.vue';
export default {
  components: {
    Navbar,
    Footer
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

  <section class="hero home is-fullheight">
    <div class="hero-head">
      <Navbar></Navbar>
    </div>
    <div class="hero-body">
      <div class="container ">
        <div class="columns is-desktop is-vcentered">
          <div class="column is-half">
            <div class="left-line"></div>
            <div id="title-text" class="dark-purple-color">
              Let's<br />
              Build Something Awesome
            </div>
          </div>
          <div class="column">
            <div class="container skill-box-wrapper">
              <RouterLink to="/projects">
                <div class="box skills-box-second">
                  <p class="title-text dark-purple-color">
                    Projects
                  </p>
                  <p>
                    <br>
                  </p>
                  <p class="subtitle slightly-light-purple-color has-text-centered">
                    <u>Checkout the projects I've worked upon.</u>
                  </p>

                </div>

              </RouterLink>
              <RouterLink to="/skills">
                <div class="box skills-box">
                  <p class="title-text dark-purple-color">
                    Skills
                  </p>
                  <u class="slightly-light-purple-color">
                    <p class="subtitle slightly-light-purple-color">
                      Find out,<br>
                      How can I<br>
                      help your<br>
                      organization.
                    </p>

                  </u>

                </div>
              </RouterLink>

            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
<Footer></Footer>

</template>

<style scoped>
.dark-purple-color {
  color: #0E5E6F;
}

.slightly-light-purple-color {
  color: #3A8891
}

#title-text {
  /* Let’s Build Something Awesome */

  font-family: 'Roboto';
  font-style: normal;
  font-weight: 600;
  font-size: 5rem;
  padding-left: 3rem;

}

.home {
  height: 100vh;
  background-color: #FFF4DF;
}

.skills-box {
  position: relative;
  top: -200px;
  background-color: #FDF5E8;
  aspect-ratio: 1;
  width: 300px;
  font-size: 4rem;

}

.skills-box-second {
  position: relative;
  z-index: 1;
  top: 200px;
  left: 170px;
  background-color: #FFF2DB;
  aspect-ratio: 1;
  width: 300px;
  font-size: 4rem;
}

.skill-box-wrapper {
  width: 450px;
}


@media screen and (min-width:1024px) {
  #title-text {
    /* Let’s Build Something Awesome */

    font-family: 'Roboto';
    font-style: normal;
    font-weight: 600;
    font-size: 6.5rem;
    color: #0E5E6F;
    padding-left: 3rem;

  }

  .home {
    height: 100%;
    background: linear-gradient(90deg, #FFF4DF 50%, #ffffff 50%);
  }

  .left-line {
    position: absolute;
    z-index: 3;
    left: 1.5rem;
    top: 7rem;
    width: 0%;
    height: 90%;
    border: 4px solid #0E5E6F;
  }
}
</style>