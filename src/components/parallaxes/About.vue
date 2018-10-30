<template>
    <v-parallax class="parallax" :src="require('@/assets/rusticlaptop.jpg')">
        <v-layout
            align-center
            justify-center
        >
            <h1 class="intro font-weight-regular text-no-wrap">
                I'm Sylum Mastropaolo
            </h1>
        </v-layout>
    </v-parallax>
</template>

<script>
export default {

}
</script>

<style>
.parallax {
  min-height: 70vmin;
  max-height: 70vmin
}
</style>
