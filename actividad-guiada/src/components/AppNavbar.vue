<template>
    <nav class="navbar navbar-expand-lg bg-azulito">
        <div class="container">
      <a class="navbar-brand col-2" href="#"><img class="logo-chefcito" :src="chefcito"></a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav ms-auto">
        <a class="nav-link fs-3" aria-current="page" href="#">{{ nav1 }}</a>
        <a class="nav-link fs-3" href="#">{{ nav2 }}</a>
        <a class="nav-link fs-3" href="#">{{ nav3 }}</a>
        
      </div>
    </div>
  </div>
</nav>

</template>

<script setup>
import { ref } from 'vue'
const nav1 = ref('Inicio')
const nav2 = ref('Nuestros platos')
const nav3 = ref('Contacto')

import chefcito from '@/assets/img/chefcito.png'
</script>

<style scoped> 
.navbar{
    background-color: darkblue;
}
a{
    color: white;
}

.logo-chefcito{
    width: 30%;
}
</style>