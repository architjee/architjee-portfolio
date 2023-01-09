<template>

    <div class="container">
        <div class="columns">
            <div class="column is-5">

            </div>
            <div class="column is-half">
                <div class="card">
                    <header class="card-header">
                        <p class="card-header-title">
                            Programming Languages
                        </p>
                    </header>
                    <div class="card-content">
                        <div class="content">
                            <div class="columns is-vcentered">
                                <div class="column is-8 has-text-left">
                                    <div class="is-size-5">
                                        59th Rank in Online Hackathon Festival
                                    </div>
                                    <div class="is-size-6 has-text-grey-light">
                                        Among 6700+ teams. Organized by Dare2Compete
                                    </div>
                                    <div class="is-size-5">
                                        Certificate of Excellence in Hack-e-Codifier
                                    </div>
                                    <div class="is-size-6 has-text-grey-light	">
                                        Organized by NIT Hamirpur </div>
                                    <div class="is-size-5">
                                        Certificate of Excellence in Dare2CODEX
                                    </div>
                                    <div class="is-size-6 has-text-grey-light	">
                                        Organized by NIT Rourkela
                                    </div>
                                    <div class="is-size-5">
                                        Certificate of Excellence in TeenHacks
                                    </div>
                                    <div class="is-size-6 has-text-grey-light	">
                                        Organized by NIT Arunachal Pradesh
                                    </div>
                                    <div class="is-size-5">
                                        Qualified NSEA and NSEC
                                    </div>
                                    <div class="is-size-6 has-text-grey-light	">
                                        Organized by IAPT
                                    </div>
                                </div>
                                <div class="column is-4">
                                    <img src="../assets/Trophyicon.svg">
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
import ProgressBar from '../components/ProgressBar.vue';

export default {
    components: {
        'my-progress-bar': ProgressBar,

    },
    data() {
        return {

        }
    },

}
</script>
<style scoped>
.container {
    min-height: 80vh;
}
</style>