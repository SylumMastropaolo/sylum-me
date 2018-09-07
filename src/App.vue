<template>
  <v-app dark>
    <v-parallax class="parallax" :src="require('@/assets/rusticlaptop.jpg')">
      <v-layout
        align-center
        justify-center
      >
        <h1
          class="intro font-weight-regular text-no-wrap"
        >I'm Sylum Mastropaolo</h1>
      </v-layout>
    </v-parallax>
    <v-layout row wrap justify-center>
      <v-btn flat v-for="link in links" :key="link.name" @click="page = link.page">
        {{link.name}}
      </v-btn>
    </v-layout>
    <v-content class="content">
      <component :is="page"></component>
    </v-content>
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
.intro {
  font-size: 8vw
}
.parallax {
  min-height: 70vmin;
  max-height: 70vmin
}
.content {
  min-height: 70vh
}
</style>
