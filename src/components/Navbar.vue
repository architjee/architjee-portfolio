
<template>
    <nav class="navbar">
        <div class="container">
            <div id="navMenu" class="navbar-menu">
                <div class="navbar-start">
                    <RouterLink to="/" class="navbar-item is-size-5 has-text-weight-semibold	">Archit Jain</RouterLink>
                </div>
                <div class="navbar-end">
                    <RouterLink to="/" class="navbar-item">Home</RouterLink>
                    <RouterLink to="/skills" class="navbar-item">Skills</RouterLink>
                    <div class="navbar-item">
                        <div class="buttons">
                            <a class="button is-dark" href="https://github.com/architjee"  target="_blank">Github</a>
                            <a class="button is-link" :href="resume" download>Download</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>


</template>

<script>
import resumeURL from '../assets/Archit_Jain_Resume.pdf'
export default {
  data() {
    return {
      resume: resumeURL
    }
  }
}

</script>