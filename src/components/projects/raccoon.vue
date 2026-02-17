<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/raccoon.png"
            alt="Raccoon Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Risk Communication </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                Risk Communication
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/raccoon.png"
                    alt="Raccoon Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://akleinau.github.io/raccoon/"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://akleinau.github.io/raccoon/
                    </a>
                </v-sheet>
                <div class="description">
                    I developed this project as part of my master thesis and PhD to support risk communicators 
                    in both extracting risk factors from their epidemiological data sets as well as 
                    visualizing them for diverse audiences. It supports diverse adaptations of the
                     visualizations to a specific user group, including visualization formats, color,
                     style, text and fonts.
                </div>
                <v-btn
                    class="mt-4"
                    variant="outlined"
                    prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/raccoon"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    Source code
                </v-btn>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
