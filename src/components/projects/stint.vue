<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/stint.png"
            alt="stint Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Interaction Stories </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                Interaction Stories
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/stint.png"
                    alt="stint Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://akleinau.github.io/Stint/"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://akleinau.github.io/Stint/
                    </a>
                </v-sheet>
                <div class="description">
                    I created this project after developing the feature interactions project also included
                     in this portfolio. This project aims to explain feature interactions to domain experts 
                     who know a lot about their specific model or data set but not about the intricacies of AI.
                      It uses visualization and storytelling, as well as a new algorithm to compute feature
                       interactions.
                    </div>
                <v-btn
                    class="mt-4"
                    variant="outlined"
                    prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/stint"
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
