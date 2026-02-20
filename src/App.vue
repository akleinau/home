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

			<v-card class="section-menu-card" >
				<nav class="section-menu" aria-label="Page sections">
					<a href="#portfolio" class="section-link">Portfolio</a>
					<a href="#academic" class="section-link">Academic Career </a>
					<a href="#cv" class="section-link">Curriculum Vitae </a>
				</nav>
			</v-card>

			<section id="portfolio" class="anchor-section">
	      			<Portfolio />
			</section>
			<section id="academic" class="anchor-section">
				<Academic />
			</section>
			<section id="cv" class="anchor-section">
				<Cv />
			</section>
		</v-main>
	</v-app>
</template>

<style scoped>
.section-menu-card {
	width: 100%;
	max-width: 800px;
	margin: 0 auto 24px;
	background: #fff;
	border: none;
	box-shadow: none;
}

.section-menu {
	display: flex;
	width: 100%;
	background: #fff;
}

.section-link {
	flex: 1;
	padding: 14px 16px;
	text-align: center;
	text-decoration: none;
	color: #2a0448;
	font-weight: 700;
	position: relative;
	transition: background-color 0.2s ease;
}

.section-link:hover {
	background-color: #f5f0ff;
}

.section-link:not(:last-child)::after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	transform: translateY(-50%);
	height: 65%;
	border-right: 3px solid #868686;
}

.anchor-section {
	scroll-margin-top: 16px;
}

</style>
