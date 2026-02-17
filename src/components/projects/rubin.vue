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
                <div class="description">Short description goes here.</div>
                <v-btn
                    class="mt-4"
                    variant="outlined"
                    prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/RUBIN"
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
