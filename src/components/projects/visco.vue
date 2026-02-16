<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <v-img
            src="/visco.jpg"
            alt="visco Project"
            height="110"
            cover
        />
        <v-card-title>COVID Dashboard </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                VisCo Project
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <v-img
                    src="/visco.jpg"
                    alt="visco Project"
                    height="420"
                    contain
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://akleinau.github.io/visco/"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://akleinau.github.io/visco/
                    </a>
                </v-sheet>
                <div class="description">Short description goes here.</div>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
