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
                oeo Project
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/oeo.png"
                    alt="oeo Project"
                    height="420"
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
                <div class="description">Short description goes here.</div>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
