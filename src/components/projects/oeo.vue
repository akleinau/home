<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/oeo.png"
            alt="oeo Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>OEO Ontology </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                OEO Ontology
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/oeo.png"
                    alt="oeo Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://github.com/OpenEnergyPlatform/ontology"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://github.com/OpenEnergyPlatform/ontology
                    </a>
                </v-sheet>
                <div class="description">
                   This project is a little bit different to the data and interface projects I mainly focus on 
                   in this portfolio; however, working on this project was highly impactful to my career.
                    It was the first time working in an interdisciplinary team 
                    in the role of the computer scientist. I learned so much from this project and want
                     to give it a little shoutout here. As a team, or more likely as a community, 
                     we developed an ontology for the energy systems sector as part of the OpenEnergyPlatform (OEP). 
                     Please check it out if you come from that domain or are interested in ontologies. 
                </div>
                <div class="d-flex ga-2 mt-4 flex-wrap">
                    <v-btn
                        variant="outlined"
                        prepend-icon="mdi-file-code"
                        href="https://github.com/OpenEnergyPlatform/ontology"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        Source code
                    </v-btn>
                    <v-btn
                        variant="flat"
                        color="blue-darken-1"
                        prepend-icon="mdi-link-variant"
                        href="https://github.com/OpenEnergyPlatform"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        Part of OEP
                    </v-btn>
                </div>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
