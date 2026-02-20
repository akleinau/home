<script setup lang="ts">
import Portfolio from './components/portfolio.vue';
import Profile from './components/profile.vue';
import Academic from './components/academic.vue';
import Cv from './components/cv.vue';


</script>

<template>
	<v-app>
		<v-main class="pb-10">
			<Profile />
      		<Portfolio />
			<Academic />
			<Cv />
		</v-main>
	</v-app>
</template>

<style scoped>

</style>
