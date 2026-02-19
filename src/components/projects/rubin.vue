<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/rubin.png"
            alt="Rubin Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Rubin CDSS </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                Rubin CDSS
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/rubin.png"
                    alt="Rubin Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://akleinau.github.io/RUBIN/"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://akleinau.github.io/RUBIN/
                    </a>
                </v-sheet>
                <div class="description">
                    For this project, we developed a clinical decision support system that can be both 
                    made highly specific and adaptive to a specific scenario, like endometrial cancer therapy,
                     and stay flexible and generalizable to other scenarios. 
                    It is part of the endorisk project and is currently in clinical trial in multiple Dutch hospitals. 
                </div>
                <div class="d-flex ga-2 mt-4 flex-wrap">
                    <v-btn
                        variant="outlined"
                        prepend-icon="mdi-file-code"
                        href="https://github.com/akleinau/RUBIN"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        Source code
                    </v-btn>
                    <v-btn
                        variant="flat"
                        color="blue-darken-1"
                        prepend-icon="mdi-link-variant"
                        href="https://endorisk.eu"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        Part of Endorisk
                    </v-btn>
                </div>
                <div class="mt-8">
                    <h3>Publication</h3>
                    <div class="citation">
                        Kleinau, A., Mo, A., Mueller-Sielaff, J., Pijnenborg, J. M., Lucas, P. J., & Oeltze-Jafra, S. (2021). User-Centered Development of a Clinical Decision Support System. In SMARTERCARE@ AI* IA (pp. 67-78).
                    </div>
                </div>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
