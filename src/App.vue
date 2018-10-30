<template>
  <v-app dark>
    <v-layout row wrap justify-center>
      <v-btn flat v-for="link in links" :key="link.name" @click="page = link.page">
        {{link.name}}
      </v-btn>
    </v-layout>
      <router-view></router-view>
    <v-footer>
      <span>&copy; 2018</span>
    </v-footer>
  </v-app>
</template>

<script>
import About from './views/About.vue'
import Education from './views/Education.vue'

export default {
  name: 'App',
  data () {
    return {
      page: "about-me",
      links: [
        {
          name: "About Me",
          page: "about-me"
        },
        {
          name: "Education",
          page: "education"
        },
        {
          name: "Skills",
          page: ""
        },
        {
          name: "Technology",
          page: ""
        },
        {
          name: "Resume",
          page: ""
        },
        {
          name: "Projects",
          page: ""
        }
      ]
    }
  },
  components: {
    "about-me": About,
    "education": Education
  }
}
</script>

<style>
</style>
