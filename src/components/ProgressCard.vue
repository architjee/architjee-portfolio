<template>

<div class="container">
        <div class="columns">
            <div class="column is-1">

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
.container{
    top: 200px;
    min-height: 80vh;
}

</style>