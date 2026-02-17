<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/FractalSquirrel.png"
            alt="FractalSquirrel Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Fractal Squirrel</v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                Fractal Squirrel
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/FractalSquirrel.png"
                    alt="FractalSquirrel Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://akleinau.github.io/FractalSquirrel/"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://akleinau.github.io/FractalSquirrel/
                    </a>
                </v-sheet>

                <div class="description">
                    Ever wanted to run around in a fractal? Just click left or right on the screen. 
                    This was a little weekend project. Cute, buggy, and fun.
                </div>
                
                <v-btn class="mt-4" variant="outlined" prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/FractalSquirrel"
                    target="_blank" rel="noopener noreferrer">
                    Source code
                </v-btn>

            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
