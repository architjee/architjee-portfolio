
<template>
    <nav class="navbar">
        <div class="container">
            <div class="navbar-brand">
                <!-- navbar items, navbar burger... -->
                <div class="navbar-item">
                    <RouterLink to="/" class="navbar-item is-size-5 has-text-weight-bold">Archit Jain</RouterLink>
                </div>
                <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false"
                    data-target="navbarBasicExample" @click="toggle_burger" :class="{'is-active': burgermenustatus}">
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                </a>
            </div>
            <div id="navMenu" class="navbar-menu" :class="{'is-active': burgermenustatus}">
               

                <div class="navbar-end external-links">
                    <RouterLink to="/" class="navbar-item">Home</RouterLink>
                    <RouterLink to="/skills" class="navbar-item">Skills</RouterLink>
                    <div class="navbar-item">
                        <div class="buttons">
                            <a class="button is-dark" href="https://github.com/architjee" target="_blank">
                                <span class="icon is-small"><i class="bi bi-github"></i></span>
                                <span>
                                    Github
                                </span>
                            </a>
                            <a class="button is-link" :href="resume" download>
                                <span class="icon is-small"><i class="bi bi-cloud-arrow-down-fill"></i></span>
                                <span>
                                    Resume
                                </span>

                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>


</template>

<script>
import resumeURL from '../assets/Archit_Jain_Resume.pdf';

export default {
    data() {
        return {
            resume: resumeURL,
            burgermenustatus : false,
        }
    },
    methods:{
        toggle_burger(){
            this.burgermenustatus = !this.burgermenustatus;
        }
    }
}

</script>