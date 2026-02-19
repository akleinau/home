<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/smoking.png"
            alt="smoking Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Smoking Cessation </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                Smoking Cessation
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/smoking.png"
                    alt="smoking Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://pred.hbcptools.org"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://pred.hbcptools.org
                    </a>
                </v-sheet>
                <div class="description">
                    In this project, I created an interface for the AI model of my colleagues that
                     helps decision-makers decide which interventions are best suited to reduce 
                     smoking rates in their community. It is part of the Human Behaviour Change Project (HBCP). 

                </div>
                <div class="d-flex ga-2 mt-4 flex-wrap">
                    <v-btn
                        variant="outlined"
                        prepend-icon="mdi-file-code"
                        href="https://github.com/akleinau/interventions"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        Source code
                    </v-btn>
                    <v-btn
                        variant="flat"
                        color="blue-darken-1"
                        prepend-icon="mdi-link-variant"
                        href="https://www.humanbehaviourchange.org/prediction"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        Part of HBCP
                    </v-btn>
                </div>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
