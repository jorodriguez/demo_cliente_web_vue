<template>
 <div class="usuario">
 <h2> {{mensaje}} </h2>

<button @click="cargarUsuarios()"> Cargar usuarios </button>

 <table class="table table-dark">
    <tr>
        <td>Nombre</td>        
        <td>Edad</td>
        <td>Correo</td>
        <td>Clave</td>
    </tr>
    <tr v-for="usuario of listaUsuario">
        <td>{{usuario.nombre}}</td>
        <td>{{usuario.edad}}</td>
        <td>{{usuario.correo}}</td>
        <td>{{usuario.password}}</td>
    </tr>
    </tr>
 </table>

 </div>
</template>

<script src="../controllers/usuarioController.js"></script>

<style scoped>


</style>


