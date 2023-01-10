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
    <a href="../assets/BulmaIconBlack1.svg"></a>
</template>

<script>
import Badge from './Badge.vue';
import bulmaurl from '../assets/BulmaIconBlack1.svg';
import KerasURL from '../assets/Keras_logo1.svg';
import SupabaseURL from '../assets/Supabasecustomicon.svg'
import TensorflowURL from '../assets/Tensorflow_logo1.svg'
import BootstrapURL from '../assets/bootstrap-fill1.svg'
import GitURL from '../assets/git-branch-outline1.svg'
import ElectronURL from '../assets/logo-electron1.svg'
import FigmaURL from '../assets/logo-figma1.svg'
import FirebaseURL from '../assets/logo-firebase1.svg'
import MySQLURL from '../assets/mysql-icon1.svg'
import StreamlitURL from '../assets/streamlit-mark-dark1.svg'
import VueURL from '../assets/vuejs-icon1.svg'





var logos = {
    'Bulma': bulmaurl,
    'Keras': KerasURL,
    'Supabase': SupabaseURL,
    'Tensorflow': TensorflowURL,
    'Bootstrap':BootstrapURL,
    'Git': GitURL,
    'Electron': ElectronURL,
    'Figma': FigmaURL,
    'Firebase': FirebaseURL,
    'MySQL': MySQLURL,
    'Streamlit':StreamlitURL,
    'Vue.js': VueURL,
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
    min-height: 60vh;
}
.container .columns{
    top: 40vh;
}
</style>