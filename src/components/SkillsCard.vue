<template>

    <div class="container">
        <div class="columns ">
            <div class="column is-5">

            </div>
            <div class="column is-half">
                <div class="card">
                    <header class="card-header">
                        <p class="card-header-title">
                            Libraries Frameworks and Tools
                        </p>
                    </header>
                    <div class="card-content">
                        <div class="content">
                            <div class="columns is-2 is-multiline ">

                                <div v-for="logo in Object.keys(logos)" class="column is-3">
                                    <my-badge :name="logo">
                                        <template v-slot:icon>
                                            <img :src="logos[logo]">
                                        </template>
                                    </my-badge>
                                </div>


                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
import Badge from './Badge.vue';
var logos = {
    'Bulma': '../src/assets/Bulma Icon Black 1.svg',
    'Keras': '../src/assets/Keras_logo 1.svg',
    'Supabase': '../src/assets/Supabase custom icon.svg',
    'Tensorflow': '../src/assets/Tensorflow_logo 1.svg',
    'Bootstrap': '../src/assets/bootstrap-fill 1.svg',
    'Git': '../src/assets/git-branch-outline 1.svg',
    'Electron': '../src/assets/logo-electron 1.svg',
    'Figma': '../src/assets/logo-figma 1.svg',
    'Firebase': '../src/assets/logo-firebase 1.svg',
    'MySQL': '../src/assets/mysql-icon 1.svg',
    'Streamlit': '../src/assets/streamlit-mark-dark 1.svg',
    'Vue.js': '../src/assets/vuejs-icon 1.svg',
}
export default {
    components: {
        'my-badge': Badge,
    },
    data() {
        return {
            logos: logos
        }
    },

}
</script>
<style scoped>
.container {
    min-height: 80vh;
}
.container .columns{
    top: 40vh;
}
</style>