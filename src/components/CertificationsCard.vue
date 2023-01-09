<template>

    <div class="container">
        <div class="columns">
            <div class="column is-1">
            </div>
            <div class="column is-half">
                <div class="card">
                    <header class="card-header">
                        <p class="card-header-title">
                            Certifications
                        </p>
                    </header>
                    <div class="card-content">
                        <div class="content columns is-vcentered">
                            <div class="column">
                                <div class="container-of-image">
                                    <img src="../assets/DeepLearningCertification.png" alt="Snow" style="width:100%;">

                                    <div class="centered has-text-dark">Neural Networks and Deep Learning</div>
                                </div>
                            </div>
                            <div class="column">
                                <div class="container-of-image">
                                    <img src="../assets/OOPSCertification.png" alt="Snow" style="width:100%;">

                                    <div class="centered has-text-dark">Object-Oriented Data Structures in C++</div>
                                </div>
                            </div>
                            <div class="column">
                                <div class="container-of-image">
                                    <img src="../assets/UdemyAdvancedJSCertificate.png" alt="Snow"
                                        style="width:100%;">

                                    <div class="centered has-text-dark">Modern JavaScript (Udemy)</div>
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


export default {
    components: {


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


/* Container holding the image and the text */
.container-of-image {
    position: relative;
    text-align: center;
    color: white;
}


/* Centered text */
.centered {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>