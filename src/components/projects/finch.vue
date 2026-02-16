<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <v-img
            src="/finch.png"
            alt="finch Project"
            height="110"
            cover
        />
        <v-card-title>Feature Interactions </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                finch Project
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <v-img
                    src="/finch.png"
                    alt="finch Project"
                    height="420"
                    contain
                />
                <v-sheet class="url-field" rounded>
                    <a
                        class="url-link"
                        href="https://huggingface.co/spaces/hztn/finch"
                        target="_blank"
                        rel="noopener noreferrer"
                    >
                        https://huggingface.co/spaces/hztn/finch
                    </a>
                </v-sheet>
                <div class="description">Short description goes here.</div>
            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
