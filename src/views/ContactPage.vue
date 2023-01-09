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
            abilities_const: ['a Data Science Enthusiast,', 'a Software Developer,', 'working with Web Technologies,', 'also sometimes doing Game development too.']
        }
    },

}
</script>

<template>

    <section class="hero is-fullheight">
        <!-- Hero head: will stick at the top -->
        <div class="hero-head">
            <Navbar></Navbar>
        </div>
        <div class="hero-body">
            <div class="container columns is-full is-vcentered">
                <div class="column">
                    <img src="../assets/contactmephoto.png" alt="Archit Jain photograph">
                </div>
                <div class="column contact-details-column has-text-centered">
                    <p class="subtitle">

                        <span class="icon-text">
                            <span class="icon">
                                <img src="../assets/telephone.svg">
                            </span>
                            <span> +91 8085588896</span>
                        </span>

                    </p>
                    <p class="subtitle">


                        <span class="icon-text">
                            <span class="icon">
                                <img src="../assets/contact_mail.svg">
                            </span>
                            <span> architjee@gmail.com</span>
                        </span>
                    </p>
                    <p class="subtitle">
                        <a href="https://github.com/architjee">
                            <span class="icon-text">
                                <span class="icon">
                                    <img src="../assets/github.svg">
                                </span>
                                <span> https://github.com/architjee</span>
                            </span>

                        </a>
                    </p>



                </div>
            </div>

        </div>
    </section>
    <Footer></Footer>

</template>
<style scoped>
img {
    width: 50vh;
    aspect-ratio: initial;
}

</style>
