<template>

    <div class="column is-4">

        <div class="card">
            <header class="card-header">
                <p class="card-header-title">
                    <a :href="link" class="has-text-black"> 
                        {{ title }}
                    </a>
                </p>
                <button class="card-header-icon" aria-label="more options">
                    <span class="icon">
                        <i class="fas fa-angle-down" aria-hidden="true"></i>
                    </span>
                </button>
            </header>
            <div class="card-content">
                <div class="content">
                    <div class="card-image">
                        <figure class="image">
                            <img :src="imagelink" :alt="title">
                        </figure>
                    </div>
                </div>
                <div class="content has-text-left">
                    <ul>
                        <li v-for="subtext in content">
                            {{ subtext }}
                        </li>


                    </ul>
                    <p>
                        <span v-for="tag in tags">
                            •
                            <span class="tag is-light" :class="randColor()">{{ tag }} </span>
                        </span>
                    </p>
                    <a :href="link">{{ link }}</a>
                    <br>
                    <time class="has-text-grey">{{ dateslot }}</time>
                </div>
            </div>
            <footer class="card-footer">


            </footer>
        </div>


    </div>
</template>
<script >
export default {
    props: ['link', 'title', 'content', 'imagelink', 'dateslot', 'tags'],
    data() {
        return {

        }
    },
    methods: {
        randColor() {

            let colors_array = ["is-black", "is-light",  "is-primary", "is-link", "is-info", "is-success", "is-warning", "is-danger"];

            return colors_array[Math.floor(Math.random() * colors_array.length)]
        }

    },
    mounted() {

    }
}
</script>
<style scoped>
.image img {
    height: 150px;
    aspect-ratio: initial;
}
</style>