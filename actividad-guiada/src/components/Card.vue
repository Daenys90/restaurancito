<template>
      <img :src="imagen" class="card-img-top" :alt="titulo">
                <div class="card-body">
                    <h5 class="card-title">{{ titulo }}</h5>
                    <p class="card-text">{{ descripcion }}</p>
                    <a href="#" class="btn btn-primary">{{ botonTarjeta }}</a>
                </div>
</template>

<script setup>
import { ref } from 'vue'

const botonTarjeta = ref("Detalles")

defineProps({
    imagen: String,
    titulo: String,
    descripcion: String
})

</script>

<style scoped>


</style> 