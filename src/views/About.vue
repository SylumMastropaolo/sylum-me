<template>
  <v-container fluid fill-height>
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
          <div class="display-1">
            I'm a fancy pants programmer who doesn't have fancy pants because he doesn't have a fancy pants job yet.
          </div>
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
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
