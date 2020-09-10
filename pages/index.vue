<template>
  <h1>
    Welcome to develop nuxtjs
  </h1>
</template>
<script>
export default {
  //en esta seccion se añaden las etiquetas meta
    head(){
      return{
        //titulo de la pagina
        title:'Bienvenido | despliegue de articulos',
        //meta atributos
        meta:[
          {
            hid:"description",
            name:"description",
            content:"Pagina de prueba de nuxt con publicaciones"
          }
        ],
        //Atributos html
        htmlAttrs:{
          lang: 'es'
        }
      }
    }
}
</script>