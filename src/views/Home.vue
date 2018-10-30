<template>
        <v-layout column>
            <v-flex xs12 md8>
                <about-parralax></about-parralax>
                <about-me></about-me>
                <education-parralax></education-parralax>
                <education></education>
            </v-flex>
        </v-layout>
</template>

<script>
import AboutParallax from "@/components/parallaxes/About.vue"
import About from "./About.vue";
import EducationParallax from "@/components/parallaxes/Education.vue"
import Education from "./Education.vue";

export default {
  components: {
    "about-parralax": AboutParallax,
    "about-me": About,
    "education-parralax": EducationParallax,
    "education": Education
  }
};
</script>

<style>
.intro {
  font-size: 8vw
}
</style>
