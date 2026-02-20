<script setup lang="ts">
const scholarUrl = 'https://scholar.google.com/citations?user=fbk005oAAAAJ&hl=de&oi=ao'
</script>

<template>
	<v-card class="mx-auto mt-6" max-width="800">
		<v-card-text class="d-flex align-center justify-space-around ">

			<v-btn
				variant="outlined"
				class="academic-btn"
				:href="scholarUrl"
				target="_blank"
				rel="noopener noreferrer"
			>
				Academic profile here
            </v-btn>
		</v-card-text>
	</v-card>
</template>

<style scoped>


.academic-btn {
	font-size: 1.1rem;
	color: #000 !important;
	border-color: #000 !important;
}
</style>
