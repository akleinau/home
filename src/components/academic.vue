<script setup lang="ts">
const scholarUrl = 'https://scholar.google.com/citations?user=fbk005oAAAAJ&hl=de&oi=ao'
</script>

<template>
	<v-card class="mx-auto mt-6" max-width="800">
		<v-card-title>
            <h3>Academic Career</h3>
           <div class="text-grey-darken-2 text-wrap" style="font-size: 1rem;">
                In my PhD, I focus on clinical decision support systems, specifically how XAI can be used inside them, especially with feature interactions. 
           </div>

        </v-card-title>

		<v-card-text>


			<div class="academic-btn-row">
				<v-btn
					variant="outlined"
					class="academic-btn"
					:href="scholarUrl"
					target="_blank"
					rel="noopener noreferrer"
				>
					Academic profile here
            	</v-btn>
			</div>
		</v-card-text>
	</v-card>
</template>

<style scoped>


.academic-btn {
	font-size: 1.1rem;
	color: #000 !important;
	border-color: #000 !important;
}

.academic-text {
	margin: 0 0 16px;
}

.academic-btn-row {
	display: flex;
	justify-content: center;
}
</style>
