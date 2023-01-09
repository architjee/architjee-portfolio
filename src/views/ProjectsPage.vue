<script >
import ProgressBar from '../components/ProgressBar.vue';
import Navbar from '../components/Navbar.vue';
import Abilities from '../components/Abilities.vue';
import ProjectCard from '../components/ProjectCard.vue';
import Footer from '../components/Footer.vue';
import TableURL from '../assets/table.svg';
import BrainURL from '../assets/Vector.svg';
import ChestURL from '../assets/Vector2.svg'
import ChatURL from '../assets/forum_FILL0_wght400_GRAD0_opsz48 2.svg'
var Thumbnails = { TableURL, BrainURL, ChestURL, ChatURL }
export default {
    components: {
        'my-progress-bar': ProgressBar,
        Navbar,
        Abilities,
        ProjectCard,
        Footer
    },
    data() {
        return {
            Thumbnails: Thumbnails,
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
                <div class="columns is-multiline">

                    <ProjectCard title="Sheets Clone" link="https://kutt.it/sheetsclone"
                        :imagelink="Thumbnails.TableURL" dateslot="November 2022"
                        :tags="['Supabase', 'Vue.js', 'Pinia']"
                        :content="['State management implemented using Pinia', 'Routing enabled using the ‘vue-router’', 'With Backend and authentication powered by Supa Base.']">
                    </ProjectCard>

                    <ProjectCard title="Brain Tumor Classification and WebApp" link="https://kutt.it/brainapp"
                        :imagelink="Thumbnails.BrainURL" dateslot="January 2021"
                        :content="['MRI Brain Tumor dataset of 2k images', 'Multiclass classification using Transfer Learning', 'Using Advanced models as MobileNet, EfficientNetB0',]"
                        :tags="['Keras', 'Tensorflow', 'Streamlit']"></ProjectCard>

                    <ProjectCard title="Pneumonia Detection (CXR)" link="https://kutt.it/pneumonia"
                        :imagelink="Thumbnails.ChestURL" dateslot="November 2020"
                        :content="['Chest X-ray’s kaggle dataset (5k+ images).', 'Binary Classification of CXRs using CNN and VGG16 with validation accuracy of 93', 'Functional API of Tensorflow']"
                        :tags="['Keras', 'Tensorflow', 'Streamlit']">
                    </ProjectCard>


                    <ProjectCard title="Chatroom Project" link="https://kutt.it/chatroom"
                        :imagelink="Thumbnails.ChatURL" dateslot="February 2020"
                        :content="['Real-time messaging web app', 'Used Firestore and Firebase as a backend', 'Responsive Front-End design']"
                        :tags="['Bootstrap', 'Firebase-Firestore', 'Javascript']">
                    </ProjectCard>

                </div>
            </div>
        </div>
    </section>


    <Footer></Footer>

</template>

<style scoped>

</style>