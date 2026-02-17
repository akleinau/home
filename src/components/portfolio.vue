<script setup lang="ts">
import Finch from './projects/finch.vue';
import Raccoon from './projects/raccoon.vue';
import Rubin from './projects/rubin.vue';
import Stint from './projects/stint.vue';
import Visco from './projects/visco.vue';
import Oeo from './projects/oeo.vue';
import MdTeilt from './projects/mdteilt.vue';
import FractalSquirrel from './projects/fractalSquirrel.vue';
import Smoking from './projects/smoking.vue';



</script>

<template>
    <v-card class="mx-auto" max-width="800">

        <v-card-title>
           <h2>Portfolio</h2>
           <div class="text-grey-darken-2 text-wrap" style="font-size: 1rem;">
                A collection of my favorite openly available projects I have had the pleasure to work on.  
           </div>
        </v-card-title>

        <v-card-text class="align-center justify-center text-center pa-8 bg-white">

            <h1> Healthcare </h1>
            <div class="project-row d-flex">
                <Rubin />
                <Raccoon />
                <Visco />
            </div>

            <h1 class="mt-8"> XAI </h1>
            <div class="project-row d-flex">
                <Finch />
                <Stint />
                <Smoking />
            </div>

            <h1 class="mt-8"> Ontology Projects </h1>
            <div class="project-row d-flex">
                <Oeo />
            </div>

            <h1 class="mt-8"> Volunteering Projects </h1>
            <div class="project-row d-flex">
                <MdTeilt />
            </div>

            <h1 class="mt-8"> Fun Projects </h1>
            <div class="project-row d-flex">
                <FractalSquirrel />
            </div>


        </v-card-text>
    </v-card>

</template>

<style scoped>
.project-row {
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 16px;
}
</style>
