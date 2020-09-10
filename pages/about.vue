<template>
    <div>
         <h1>About us</h1>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Rem commodi quasi nam laboriosam. Quisquam, cupiditate cumque. Ea qui ab at! Tenetur voluptate quisquam quod dignissimos assumenda explicabo, sapiente iusto. Magnam.</p>
    </div>
   
</template>
<script>
export default {
    head(){
        return{
            //titulo de la pagina
        title:'Acerca de lo que se está haciendo',
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