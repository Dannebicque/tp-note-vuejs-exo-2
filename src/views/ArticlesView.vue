<template>
    <h1>Articles</h1>
    <div class="row">
        <div class="col-12">
            <h2>Liste des articles</h2>
            <div v-if="data">
                
            </div>
            <div v-else>
                <p>Chargement en cours...</p>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col-12">
            <h2>Ajouter un article</h2>
            <form>
                <label for="titre">Titre</label>
                <input type="text" id="titre" name="titre" required class="form-control">

                <label for="contenu">Contenu</label>
                <textarea id="contenu" name="contenu"  required class="form-control"></textarea>
                
                <button class="btn btn-primary">Ajouter</button>
            </form>
        </div>
    </div>
</template>

<script setup>

import { ref } from 'vue';
const data = ref(null);

</script>