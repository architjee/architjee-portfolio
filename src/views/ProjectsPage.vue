<script >
import ProgressBar from '../components/ProgressBar.vue';
import Navbar from '../components/Navbar.vue';
import Abilities from '../components/Abilities.vue';
export default {
    components: {
        'my-progress-bar': ProgressBar,
        Navbar,
        Abilities
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

        <!-- Hero content: will be in the middle -->
        <div class="hero-body">
            <div class="container has-text-centered">
                <p class="title">
                   THis is my projects page.
                </p>
            </div>
        </div>
    </section>

    <div class="container">
        <div class="columns">
            <div class="column is-half is-offset-one-quarter">
                <div class="card">
                    <header class="card-header">
                        <p class="card-header-title">
                            Programming Languages
                        </p>
                    </header>
                    <div class="card-content">
                        <div class="content">
                            <p>
                                <my-progress-bar label="Python" size="90" color="is-info"></my-progress-bar>
                            </p>
                            <p>
                                <my-progress-bar label="JavaScript" size="85" color="is-success"></my-progress-bar>
                            </p>
                            <p>
                                <my-progress-bar label="Java" size="80" color="is-primary"></my-progress-bar>
                            </p>
                            <p>
                                <my-progress-bar label="C/C++" size="80" color="is-danger"></my-progress-bar>
                            </p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>



</template>
