<script setup lang="ts">
import Raccoon from './projects/raccoon.vue';
import Rubin from './projects/rubin.vue';




</script>

<template>
    <v-card class="mx-auto" max-width="800">
        <v-card-text class="align-center justify-center text-center pa-8">

            <h1> Healthcare </h1>
            <div class="d-flex">
                <Rubin />
                <Raccoon />
            </div>


        </v-card-text>
    </v-card>

</template>

<style scoped>

</style>
