<template>
  <v-container fluid fill-height class="content">
    <v-slide-y-transition mode="out-in">
      <v-layout row justify-center align-center text-xs-center wrap>
        <v-flex xs12 md4>
          <v-avatar
            size="300px"
            class="elevation-24"
          >
            <img src="@/assets/HeadshotCropped.jpeg">
          </v-avatar>
        </v-flex>
        <v-flex xs12 md5>
          <v-layout column>
            <v-flex xs12>
              <h1 class="display-3"> About Me </h1>
            </v-flex>
            <v-flex xs12 md5>
              <div class="display-1">
                I am a programmer and have always been a programmer. I've known that I wanted to pursue a career in computer science ever since I took a one-week coding bootcamp in 9th grade. I haven't lost a single ounce of excitement or passion for it since. As I continue to grow and expand my experiences, my childlike wonder fuels my drive to learn new things and solve new problems. Programming has been and always will be my passion. I love what I do.
              </div>
            </v-flex>
          </v-layout>
        </v-flex>
      </v-layout>
    </v-slide-y-transition>
  </v-container>
</template>

<script>

export default {
  name: 'About',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.content {
  min-height: 70vh
}

</style>
