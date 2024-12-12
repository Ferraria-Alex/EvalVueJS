<template>
    <nav class="navbar navbar-dark bg-dark" aria-label="First navbar example">
        <div class="container-fluid">
            <router-link class="navbar-brand" to="/home">Logo</router-link>
            <button class="navbar-toggler collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#navbarsExample01" aria-controls="navbarsExample01" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="navbar-collapse collapse" id="navbarsExample01" style="">
                <ul class="navbar-nav me-auto mb-2">
                    <li class="nav-item">
                        <router-link class="nav-link active" aria-current="page" to="/home">Home</router-link>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script setup lang='js'>

import { RouterLink } from 'vue-router'

</script>

<style scoped lang="css">
</style>