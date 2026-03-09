<template>
<section class="container mb-5">
        <h2 class="text-center my-5 display-5 fw-normal">{{ subtitulo }}</h2>
        <div class="row gap-5 justify-content-evenly">
            <div class="col-10 col-sm-10 col-md-5 col-lg-3 p-0"
            v-for="card in cards"
            :key="card.id"
            >
                <Card 
                :imagen="card.imagen"
                :titulo="card.titulo"
                :descripcion="card.descripcion"
                />
            </div>
        </div>
</section>
<Payment />
</template>

<script setup>
import { ref } from 'vue'
import Card from './Card.vue';
import Payment from './Payment.vue';
import bebidas from '@/assets/img/bebidas.jpg'
import colaciones from '@/assets/img/colaciones.jpg'
import desayunos from '@/assets/img/desayunos.jpg'
import dulces from '@/assets/img/dulces.jpg'
import empanadas from '@/assets/img/empanadas.jpg'
import verduras from '@/assets/img/verduras.jpg'

const subtitulo = ref('Nuestros platos')
const cards = ref([
    {
        id:1,
        imagen: bebidas,
        titulo: "Bebidas",
        descripcion: "Toma bebida"
    },
    {
        id:2,
        imagen: colaciones,
        titulo: "Colaciones",
        descripcion: "Almuerzaaaa"
    },
    {
        id:3,
        imagen: desayunos,
        titulo: "Desayuno",
        descripcion: "Comienza el día"
    },
    {
        id:4,
        imagen: dulces,
        titulo: "Colaciones",
        descripcion: "Almuerzaaaa"
    },
    {
        id:5,
        imagen: empanadas,
        titulo: "Empanadas",
        descripcion: "uyuyuuuuuuui"
    },
    {
        id:6,
        imagen: verduras,
        titulo: "Verduras",
        descripcion: "Vegano y fit"
    }
])
</script>

<style scoped>


</style> 