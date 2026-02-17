<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/visco.jpg"
            alt="visco Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>COVID Dashboard </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                COVID Dashboard
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/visco.jpg"
                    alt="visco Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://akleinau.github.io/VisCo/"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://akleinau.github.io/VisCo/
                    </a>
                </v-sheet>
                <div class="description">
                    This project shows a simple COVID dashboard that I developed as part of a team project
                     during the pandemic. I include it in this portfolio because it is simple and easy to 
                     understand and not as complex as some of my other projects; however, it is
                      getting outdated by the minute. If it doesn't work anymore, I'm sorry. 
                      But I'm also glad that we don't need it anymore. 
                </div>
                <v-btn
                    class="mt-4"
                    variant="outlined"
                    prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/visco"
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
