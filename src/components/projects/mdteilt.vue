<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/mdteilt.jpg"
            alt="mdteilt Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Magdeburg teilt!</v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                mdteilt Project
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/mdteilt.jpg"
                    alt="mdteilt Project"
                    class="project-img-contain"
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://magdeburg-teilt.de"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://magdeburg-teilt.de
                    </a>
                </v-sheet>
                <div class="description">
                    We started this project to collect regular events and activities in Magdeburg that are based 
                    on Solidarity.
                </div>
                <v-btn
                    class="mt-4"
                    variant="outlined"
                    prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/mdteilt"
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
