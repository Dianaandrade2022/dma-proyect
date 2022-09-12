<script setup lang="ts">
  export default{
    data:() =>({
     contador : 500,
    }),
    methods:{
      incrementar(){
        this.contador++;
      },
      disminuir(){
        this.contador--;
      },
      reset(){
        this.contador = 500;
      },
    },
  };
</script>

<template>
    
        <!-- Button trigger modal -->
        <div class="modalcontainer">
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#staticBackdrop">
    Estudiante
  </button>
  
  <!-- Modal -->
    <div class="modal fade" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="staticBackdropLabel">Diana Martínez Andrade 4B</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
           Materia: Aplicaciones Web orientadas a servicios
           <br>
           Carrera: Desarrollo de Software Multiplataforma
          </div>
          <div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cerrar</button>
          </div>
        </div>
      </div>
    </div>
      </div>  
      <div class="containercontent">
    <img src="./assets/logo.svg" alt="" srcset="" widht="125" height="125" class="m-2">
    <h1 class="text-center text-danger">Hola desde vue.js 3</h1>
    <hr>
  <div class="m-1 text-center">
   <h2 class="text-light">Contador {{contador}}</h2>
   <button class="btn btn-light m-1" @click="incrementar()">+1</button>
   <button class="btn btn-danger m-1" @click="disminuir()">-1</button>
   <button class="btn btn-primary m-1" @click="reset()">Reset</button>
  </div>
  </div>
</template>

<style>
    img{
        box-shadow: 2px 2px 4px rgb(255, 238, 238);
    }
    hr{
        background-color: white;
        height: 3px;
    }
    h1{
      font-variant:small-caps;
      font-weight: 600;
    }
</style>

