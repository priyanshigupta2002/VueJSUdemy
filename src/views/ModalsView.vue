<template>
    <div class="modals">
        <h1>Modals</h1>
        <button @click="showModal=true">Show modal</button>
        <div v-if="showModal"
        class="modal">
            <h1>This is a modal</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus ipsa quas itaque obcaecati. Veritatis, tempore. Iste deserunt nisi saepe. Architecto nesciunt rerum ex quia corrupti. Perferendis pariatur ratione voluptatibus quaerat?</p>
            <button @click="showModal=false">Hide modal</button>
        </div>
    </div>
</template>
<script setup>
import {ref} from 'vue'
const showModal=ref(false)
</script>
<style>
.modal{
    background:beige;
    padding:10px;
}
</style>