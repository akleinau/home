<script setup lang="ts">
import { ref } from 'vue'

const dialog = ref(false)
</script>

<template>
    <v-card class="minicard" @click="dialog = true">
        <img
            src="/finch.png"
            alt="finch Project"
            height="110"
            class="project-img-cover"
        />
        <v-card-title>Feature Interactions </v-card-title>
    </v-card>

    <v-dialog v-model="dialog" max-width="900">
        <v-card class="maxicard">
            <v-card-title class="d-flex align-center justify-space-between">
                Feature Interactions
                <v-btn icon="mdi-close" variant="text" @click="dialog = false" />
            </v-card-title>
            <v-card-text>
                <img
                    src="/finch.png"
                    alt="finch Project"
                    class="project-img-contain"
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
                <div class="description">
                    This project is part of my PhD, where I looked into how feature interactions
                     can be visualized in models trained on tabular data sets. The user starts with a dataset and
                     model and then selects one feature after another, 
                     seeing how they interact.</div>
                <v-btn
                    class="mt-4"
                    variant="outlined"
                    prepend-icon="mdi-file-code"
                    href="https://github.com/akleinau/finch"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    Source code
                </v-btn>

                    <div class="mt-8">
                        <h3>Publication</h3>
                        <div class="citation">
                            Kleinau, A., Preim, B., & Meuschke, M. (2025). FINCH: Locally Visualizing Higher-Order Feature Interactions in Black Box Models. arXiv preprint arXiv:2503.16445.
                        </div>
                    </div>

            </v-card-text>
        </v-card>
    </v-dialog>
</template>

<style scoped>

</style>
