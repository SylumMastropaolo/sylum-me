<template>
  <v-container fluid fill-height>
      <v-layout row justify-center align-center text-xs-center wrap>
				<v-flex xs12 md5>
					<v-layout column>
						<v-flex xs12>
							<h1 class="display-3"> Education </h1>
						</v-flex>
						<v-flex xs12 md5>
							<div class="display-1">
								I earned my Bachelor's Degree of Science in Computer Science at State University of New Paltz
							</div>
						</v-flex>
					</v-layout>
				</v-flex>
        <v-flex xs12 md4>
          <v-avatar
            size="300px"
            class="elevation-24"
          >
            <img src="@/assets/GraduationHeadshot.jpg">
          </v-avatar>
        </v-flex>
      </v-layout>
  </v-container>
</template>

<script>
export default {

}
</script>

<style>
.content {
  min-height: 70vh
}
</style>
