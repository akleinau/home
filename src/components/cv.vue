<script setup lang="ts">
const linkedInUrl = 'https://www.linkedin.com/in/anna-kleinau-241a38236/'
</script>

<template>
	<v-card class="mx-auto mt-6" max-width="800">
        <v-card-title>
            <h3>Curriculum Vitae</h3>
           <div class="text-grey-darken-2 text-wrap" style="font-size: 1rem;">
                You can find my contact information and CV on my LinkedIn profile. 
           </div>

        </v-card-title>
        
		<v-card-text class="d-flex align-center justify-space-around ">
			<v-btn
				variant="outlined"
				class="cv-btn"
				:href="linkedInUrl"
				target="_blank"
				rel="noopener noreferrer"
			>
				Contact Info and CV here
			</v-btn>
		</v-card-text>
	</v-card>
</template>

<style scoped>
.cv-btn {
	font-size: 1.1rem;
	color: #000 !important;
	border-color: #000 !important;
}
</style>
